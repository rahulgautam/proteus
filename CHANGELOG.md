# Change log

## 0.3.7

Open source time.

## 0.3.6 ([#18](https://git.mobcastdev.com/Deployment/proteus/pull/18) 2014-11-10 12:49:23)

Use the time from when things were merged in

Patch

The changelog.md will mention the time things were merged in by Proteus and that version came to be; not the timestamp of when the PR was filed. If you want that, follow the link to the PR itself.

## 0.3.5 ([#17](https://git.mobcastdev.com/Deployment/proteus/pull/17) 2014-08-14 12:34:11)

Real regex

### Bug fix

- I'm a complete idiot and forgot to escape the hyphen.

## 0.3.4 ([#16](https://git.mobcastdev.com/Deployment/proteus/pull/16) 2014-08-14 12:24:57)

Allow dot and underscores in repo names

### Bug fix

- git repos can have dots and underscores, we need to ensure these are included!

## 0.3.3 ([#15](https://git.mobcastdev.com/Deployment/proteus/pull/15) 2014-08-04 11:13:21)

Grab a FAIL gif at random using the giphy API

### Patch

Attempt to grab a fresh, new and funny fail gif from Giphy, instead of cycling the same old images over and over

## 0.3.2 ([#14](https://git.mobcastdev.com/Deployment/proteus/pull/14) 2014-07-29 12:13:37)

Actually collect version

### Improvements

- *Actually* collect the version number from proteus, rather than pretending to, and cocking it all up.

## 0.3.1 ([#12](https://git.mobcastdev.com/Deployment/proteus/pull/12) 2014-07-29 11:56:22)

Only alter changelog and version when merging to master

### Improvements

- Ensure PRs to non-master don't commit changelog and version changes.

## 0.3.0 ([#10](https://git.mobcastdev.com/Deployment/proteus/pull/10) 2014-06-16 15:43:24)

Case statement fail!

### Bug fix

- Fixed an issue with `0.y.z` breaking changes where they would never be detected.

## 0.2.2 ([#9](https://git.mobcastdev.com/Deployment/proteus/pull/9) 2014-05-21 12:14:20)

JP, you're a tool

### Bugfix

- JP's a massive tool.

With respect,

JP

## 0.2.1 ([#8](https://git.mobcastdev.com/Deployment/proteus/pull/8) 2014-05-21 10:20:32)

Only check for banned files on PR

### Bugfixes

- Correctly only check for banned files on PR runs. (Previous implementation didn't set `@version` which broke later steps)
- Allow pull requests which *only* change `VERSION` and `CHANGELOG.md`

## 0.2.0 ([#7](https://git.mobcastdev.com/Deployment/proteus/pull/7) 2014-05-20 13:50:10)

Allow breaking changes in v0

#### New features

- When the current version is `0.y.z` then text indicating incompatible changes increments the `minor` rather than `major` version, as incompatible changes are expected in v0 products and you can make incompatible changes in v0 according to the semantic versioning policy.

## 0.1.3 ([#6](https://git.mobcastdev.com/Deployment/proteus/pull/6) 2014-05-20 11:36:52)

Allow the improvement keyword

### Improvement

- Patch to add the "improvement" keyword, it will be recognised as a PATCH version bump.



## 0.1.2 ([#5](https://git.mobcastdev.com/Deployment/proteus/pull/5) 2014-04-25 13:31:39)

Falsely detecting changes to CHANGELOG & VERSION

### Bug fixes

* Fixed a bug where Proteus was not diff-ing from the right branch to check the last upstream commit changes ([CP-1416](https://tools.mobcastdev.com/jira/browse/CP-1416))
* Changed the exit code from `1` to `3` when an exception is captured

## 0.1.1 ([#4](https://git.mobcastdev.com/Deployment/proteus/pull/4) 2014-04-24 16:03:50)

Allow underscores in repo names

### Bug fixes

- Accepts repo and owner names which have underscores in.

## 0.1.0 ([#3](https://git.mobcastdev.com/Deployment/proteus/pull/3) 2014-04-23 13:56:08)

Correct checking for banned files

### New features

- Fail gifs. Because awesome.

### Bug fix

- Correctly ascertains if you've tried to push a pull request with changes to `VERSION` or `CHANGELOG.md` files.

