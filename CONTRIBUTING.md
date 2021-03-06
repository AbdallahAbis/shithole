Welcome! First off; _**THANK YOU**_ for your interest in contributing to
Shithole! We know that your time is valuable; so let's get started!

## Ground Rules

The key words “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”,
“SHOULD NOT”, “RECOMMENDED”, “MAY”, and “OPTIONAL” in this document are to be
interpreted as described in [RFC 2119][rfc-2119].

### Contributor Ground Rules

- Contributors _must_ comply with our [code of conduct][code-of-conduct].
- Contributors _must_ [assign ownership][assign-ownership] of their
  contributions to Zinc Technology Inc (ZTI).
- Contributors _must not_ commit directly to the `development` or `production`
  branches.
- Contributors _should_ [ask for help][get-help] when they get stuck.
- Contributors _may_ build on top of other Contributors unmerged branches.

### Maintainer Ground Rules

- Maintainers _must_ comply with our [code of conduct][code-of-conduct].
- Maintainers _must_ perform regression testing prior to release.
- Maintainers _must_ ensure that all feedback provided to Contributors is
  specific, actionable, and kind.
- Maintainers _must not_ erase authorship information from any Contributors.
- Maintainers _should_ acknowledge Contributors issues and patches within two
  weeks of submission.

## How can I contribute...

### Security concerns?

We need to create a more formal responsible security disclosure process; but in
the meantime, we strongly encourage people with security concerns to [create a
ticket][issue-tracker] explaining their concerns. If the concern is a
vulnerability in a released version of compensated; please [email the
maintainers][email-maintainers].

### Documentation improvements?

Because Compensated is very early alpha software, it's light on documentation.
If you are trying to figure something out or have a question we would love for
you to [open a ticket][issue-tracker] requesting documentation improvements.

If you have an idea for what that documentation would look like, you can [use
the built in GitHub editor][editing-files-in-github] to [suggest a change using
a pull request!][creating-a-pull-request]

### Bug fixes?

We consider any gaps between what you _expected_ Shithole to do and what it
_actually did_ to be a bug. It makes it easier for us to fix things when bug
reports clearly express what was expected and what actually happened.

But don't let that stop you! We'd prefer to hear about what was surprising even
if you can't reproduce it or would like help to figure out how to communicate
the issue effectively.

If you notice something weird when working in Shithole; please [open a ticket in
our issue tracker][issue-tracker]. We'll do our best to prioritize fixing bugs
over adding features.

If you want to try squashing it yourself; we encourage you to review the
[development workflow][development-workflow].

### Features?

We are happy to continue building Shithole in the direction our current clients
and projects need it to; but we'd _love_ to hear what you wish it would do! To
make a feature request, [create an issue in our issue tracker][issue-tracker].

You can also take a stab at implementing the feature yourself! If you do, we
encourage you to [create a pull request][creating-a-pull-request] as soon as you
get started, even if it's not working yet! This makes it easier to see what is
in flight, and gives you the ability ask for help by mentioning
[@zspencer][shithole-maintainers]. We'll happily work with you to get it refined
and merged in!

## Getting Help

We have two vectors for getting help; one is through [opening a ticket in our
issue tracker][issue-tracker], where we will do our best to provide support in a
timely manner.

For businesses with greater support needs, we offer professional support at
\$250USD per hour. Support may be scheduled by [emailing
hello@zincma.de][email-maintainers].

## Development Guide

The development guide is a work in progress, and is intended to serve as a
starting point for people who would like to directly modify Shithole to fix a
bug or enhance a feature.

If you have an idea of what change you would like to make, start [learning the
system][learn-the-system]. If you are already comfortable with Shithole's
product design and architecture, you can [start working on the
change][making-a-change]. For everyone else, let's [find something to
do!][find-something-to-do]

### Find Something To Do

Look at the open tickets in our [issue tracker][issue-tracker]. Items labeled
“Help Wanted” are where we would appreciate some help. Items labeled “Good First
Issue” are where we think new contributors would be able to chip in effectively.
If there aren't any labeled with these two things; feel free to pick something
else!

Now that you've got something to do,

### Learn the System

Once you've [found something to do][find-something-to-do], you'll want to [clone
the repository][cloning-a-repository] and review the [product
design][product-documentation] and [architecture
documentation][architecture-documentation] to develop a firmer grasp of the
underlying mental models.

### Install Dependencies

[Review the dependencies that require manual installation][dependencies] and
install them.

Run `bin/setup`from the project root directory or from a module specific
directory to install dependencies which can be automatically installed.

If that doesn't work, read the source of `bin/setup` and the nearest README and
try again to get it working. Failing that, [ask for help][get-help]

### Make a Change

We encourage people to start off by writing a test that demonstrates the bug
they are attempting to fix or the use case they want to add.

Run tests with `bin/test` from the project root directory or from a module
specific directory.

Ideally, there are at least two tests, a [“unit” test and a “system”
test][unit-and-system-tests]. If you are struggling to write tests, that is OK!
You can find examples of unit tests in the `spec/unit` folder. Our system tests
are written in cucumber and live in `features` folder. If you are still stuck,
you can always [ask for help][get-help].

Once you have a test that help you feel confident you will know that the change
you made has the impact you want, dive on in to writing code! Reviewing the
[architecture documentation][architecture-documentation] and the nearest README
should get you headed in the right direction. If not, [ask for help][get-help]!

### Submit a Patch

We encourage contributors to [create a pull request][creating-a-pull-request]
early, even if the work isn't 'done' as this is the easiest way to [get the best
help][get-help]. This also makes it possible for other Contributors to build on
top of the work you've already done, instead of needing to reinvent the wheel.

We encourage Contributors to follow a branch naming schema like for bugs that
looks something like `fix/apple-iap/<words-describing-fix>`; and for features
looks something like `enhance/stripe/<words-describing-improvement>`. However,
feel free to name your branches in the way that feels most comfortable to you.

## Legal

Shithole uses a proprietary license for commercial use. This ensures we can
maintain the library and related services over the long haul, as well as gives
us the right to refuse to license to organizations who we do not want to benefit
from our labor.

### Assignment of Ownership to Zinc Technology Inc (ZTI)

In order to unambiguously own and sell Shithole as a commercial product, ZTI
must have the copyright associated with the entire project. Any intellectual
property you create which is merged must be owned by ZTI. We're not trying to be
a jerk, just trying to cover our asses. (Phrasing shamelessly lifted from
[SideKiq Pro's Commercial Collaboration
Guide][sidekiq-pro-commercial-collaboration])

Before we can merge patches, we will need you to grant us all rights to the work
you perform on Shithole to ZTI. You can do this by sending “I assign all rights,
including copyright, to any future Shithole work by myself to Zinc Technology
Inc” to [the maintainer][email-maintainers] or as a comment on your
[patch][creating-a-pull-request].

[development-workflow]: #development-guide
[find-something-to-do]: #find-something-to-do
[learn-the-system]: #learn-the-system
[install-dependencies]: #install-dependencies
[making-a-change]: #make-a-change
[get-help]: #getting-help
[assign-ownership]: #assignment-of-ownership-to-zinc-technology-inc-zti
[dependencies]: ./README.md#dependencies
[architecture-documentation]: ./README.md#architecture
[product-documentation]: ./README.md#design
[code-of-conduct]: ./CODE_OF_CONDUCT.md
[shithole-maintainers]: https://github.com/zspencer
[cloning-a-repository]:
  https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository
[creating-a-pull-request]:
  https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request
[editing-files-in-github]:
  https://help.github.com/en/github/managing-files-in-a-repository/editing-files-in-your-repository
[email-maintainers]: mailto:hello@zincma.de
[issue-tracker]: https://github.com/zinc-technology/shithole/issues
[rfc-2119]: https://tools.ietf.org/html/rfc2119
[sidekiq-pro-commercial-collaboration]:
  https://github.com/mperham/sidekiq/wiki/Commercial-collaboration
[unit-and-system-tests]:
  http://softwaretestingfundamentals.com/software-testing-levels/
