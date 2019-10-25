# git-release-note
Release note generator for github

## Description

- It print information of all PR between specified versions.
  - PR number
  - title
- It does not print for it that have not been merged using PR

## Installs

```bash
curl -O https://raw.githubusercontent.com/soranoba/git-release-note/master/git-release-note
chmod +x git-release-note
mv git-release-note /usr/local/bin/
```

## Examples

When using the [bbmustache](https://github.com/soranoba/bbmustache) repository,

```
$ git release-note v1.0.0 v1.8.0
- #40 (re-make) Allow {{.}} to appear on the top level
- #39 Official support for OTP22.0
- #35 raise error if argument on default_value_serializer is unsupported term.
- #34 Adding value serializer option to bbmustache
- #31 Add frequently asked content in README / fix typos.
- #29 Fix incompatible typespecs of some options
- #30 fix typo, write officially support version at doc.
- #27 FIX: If there are templates that do not exist, parse does not end...
- #25 Support OTP 21, and officially deprecated R16
- #23 Fix a simple typo in document and comment (contex -> context)
- #18 FIX: issue #17 : Tag lookup doesn't descend the context stack
```
