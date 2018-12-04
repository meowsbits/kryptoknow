## Spinup@Phase1

### Remote version control

| Status | Service                                                                | Cost      | Alternatives                     | Specifications                      | TODO            | Related | ? |
|--------|------------------------------------------------------------------------|-----------|----------------------------------|-------------------------------------|-----------------|---------|---|
|        | [ github.com#Team :registered: ](https://github.com/organizations/new) | $9/usr/mo | github.com#Business ($21/usr/mo) | _All_ devs should have push access+ | - [ ] namespace |         |   |

### CI pipeline

These accounts should provide admin access to all developer team members. Probably this can be accomplished thru Github x-authentication, but should be ensured.

| Status | Service                                                                          | Cost    | Alternatives | Specifications | TODO                                                       | Related | ? |
|--------|----------------------------------------------------------------------------------|---------|--------------|----------------|------------------------------------------------------------|---------|---|
|        | CircleCI - Linux                                                                 | free    |              |                |                                                            |         |   |
|        | [CircleCI - OSX ](https://circleci.com/pricing/#build-os-x)#Startup :registered: | $129/mo |              |                | - [ ] dev:build workspaces, hook up to repos we'll take on |         |   |
|        | [Appveyor](https://www.appveyor.com/pricing/)                                    | free    |              |                | _ditto_                                                    |         |   |
|        |                                                                                  |         |              |                |                                                            |         |   |

### Builds: archive tools, storage, and distribution

- Mechanism to sign and ship nightly and tagged software builds
  + needs to handle authentication schemes for storage write permissions
- Storage location/service for these archived builds
- Distribution:
  + `homebrew` forumulas (@OSX only), eg. https://github.com/ethereumproject/homebrew-classic, currently supporting go-ethereum and emerald-cli (Vault)
  + Addtionally, `snap`,`apt`, `.AppImage`, `chocolate`, `docker`, et al channels should considered as well

| Status | Service                       | Cost         | Alternatives | Specifications                              | TODO | Related | ? |
|--------|-------------------------------|--------------|--------------|---------------------------------------------|------|---------|---|
|        | Google Cloud Provider#Storage | ~$0.02/GB/mo | AWS#S3       |                                             |      |         |   |
|        | Homebrew(#OSX only)           | free         |              | needs a github repo and regular maintenance |      |         |   |


### Tooling 

| Status | Service                                                                      | Cost          | Alternatives                    | Specifications | TODO | Related | ? |
|--------|------------------------------------------------------------------------------|---------------|---------------------------------|----------------|------|---------|---|
|        | [Jetbrains IDE#Goland](https://www.jetbrains.com/go/buy/#edition=commercial) | $199/usr/year | Jetbrains IDE#Suite ($649/year) |                |      |         |   |


### Documentation infrastructure 

- Tooling for documentation generation (eg. Gitbook, Docusaurus, reathedocs.io ... -> Stev)
- Hosting for documentation (github pages, self hosted...)
- Bonus points: make code and documentation tightly coupled
- Bonus points: integrate documentation rollout with CI

### Developer-developer and developer-community communication channels 

| Status | Service                                                  | Cost           | Alternatives   | Specifications                                         | TODO | Related | ? |
|--------|----------------------------------------------------------|----------------|----------------|--------------------------------------------------------|------|---------|---|
|        | Office.com#email                                         | ?              | Protonmail     | It does email                                          |      |         |   |
|        | [Zoom#Pro](https://zoom.us/pricing)                      | $14.99/host/mo | yes please?... | All devs should be hosts                               |      |         |   |
|        | Gitter                                                   | free           |                | Public facing code-centric text-based discussion forum |      |         |   |
|        | [Slack#Pro](https://ethereumclassiclabs.slack.com/plans) | $6.67/usr/mo   |                | Searchable and always-visible history                  |      |         |   |

### Daily developer routine practices and policies 
- Stand ups? When? In person?
- Mutual time-available zones?
- Scheduled architectural and design discussions?
- Scheduled sprint routines?
- Scheduled code review sessions?

### Developer expense practices and policies 
- Standard monthly allowance for hardware and compute infrastructure costs (eg. VPS rent, hardware wallet)
- Standard allowance for "Oh, shit" hardware and compute infrastructure costs (eg. replace SSD)
- Standard allowance for do-ocracy principles and independent research (eg. buy an Arduino, make a blockchain flamethrower)

