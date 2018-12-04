__Remote version control__

- Github org (`/etclabs`, `/bestwisdom`?); Privacy: :dollar:
  + Membership at reader/writer (admin+) level for _all_ developers
  + 

__CI pipelines__

- CircleCI account (Possibly Pro account: :dollar:)
  > Handles OSX and Linux tests and builds and integrates seamlessly w/ Github

- Appveyor account (possibly Pro :dollar:)
  > Handle Windows tests and builds

These accounts should provide admin access to all developer team members. Probably
this can be accomplished thru Github x-authentication, but should be ensured.

__Builds: archive tools, storage, and distribution__

- Mechanism to sign and ship nightly and tagged software builds
  + needs to handle authentication schemes for storage write permissions
- Storage location (eg. Google CP, Amazon S3 :dollar:) for these archived builds


> _isaac_: for tagged (@semver.minor+?) builds, it would be clever to add a feature to this mechanism
> that would ensure that the tag and tagged commit (`HEAD`) was _signed_ with a GPG
> key belonging to a known and publicly registered team member credentials with adequate permissions relating to the
> development team.
>   
> https://github.com/etcdevteam/janus was a tool designed for this at ETCDEV.
> Cons of reuse:
> - it handles semver formatting and gcp uploads; a very opinionated bundle
> - the semver formatting is brittle; for example, `v.1.2.3-dirty-alpha` breaks it
> - it's own verison control and tests are ugly, incorporating an ugly git submodule scenario
> 
> Pros of reuse:
> - handles symmetric an asymmetric signatures
> - proven to work, with many implementation examples

- Distribution:
  + `homebrew` forumulas (@OSX only), eg. https://github.com/ethereumproject/homebrew-classic, currently supporting go-ethereum and emerald-cli (Vault)
  + Addtionally, `snap`,`apt`, `.AppImage`, `chocolate`, `docker`, et al channels should considered as well


__Tooling__
- ETCDEV Jetbrains IDE License set to expire tomorrow (Dec. 4 2018)
  + They've also changed their open source license offerings, and now license will be paid if developers are paid

__Documentation infrastructure__

- Tooling for documentation generation (eg. Gitbook, Docusaurus, reathedocs.io ... -> Stev)
- Hosting for documentation (github pages, self hosted...)
- Bonus points: make code and documentation tightly coupled
- Bonus points: integrate documentation rollout with CI

__Developer-developer and developer-community communication channels__

- Gitter rooms, accounts
  > These are associated by github org and repo, I believe

- Slack
- Discord

- Zoom, or another video conferencing medium

- Email (@etcdevteam/protonmail might die)

```
_isaac_: IMO this should be primary domain for team communications, for the sake of transparency and community accessibility and engagement.
This doesn't mean that all rooms should be publicly writable, but at every reasonable chance should be publicly readable.
```

__Daily developer routine practices and policies__
- Stand ups? When? In person?
- Mutual time-available zones?
- Scheduled architectural and design discussions?
- Scheduled sprint routines?
- Scheduled code review sessions?

__Developer expense practices and policies__
- Standard monthly allowance for hardware and compute infrastructure costs (eg. VPS rent, hardware wallet)
- Standard allowance for "Oh, shit" hardware and compute infrastructure costs (eg. replace SSD)
- Standard allowance for do-ocracy principles and independent research (eg. buy an Arduino, make a blockchain flamethrower)

