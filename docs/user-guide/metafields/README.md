# Security Test Meta Fields

Meta Fields can store additional data which doesnt fit into the usual field of the security test data model. It basically a string to string map / object / dictionary or howerver you would call it.

We have encountered some data values which we found paticulary usefull and standardized their format to be used in multiple places.
These values can then be used by standerdized components e.g. by the DefectDojo persistence, pefilling engagment details with information about the build server and test environment

> Note: None of these values are mandatory.

## Standard Values

### Git and Build Values

| Name         | Description                                                                                              | Example                                          |
| ------------ | -------------------------------------------------------------------------------------------------------- | ------------------------------------------------ |
| BRANCH       | Git Branch of version tested by the securityTest                                                         | `develop`                                        |
| BUILD_ID     | Reference to the Build on the Build server which triggered the security test. E.g. a id of a jenkins job | 42                                               |
| COMMIT_HASH  | Git Commit Hash of the repository currently beeing tested                                                | `a9b64b...`                                      |
| REPO         | Full Url to the Git Repository                                                                           | https://git.internal.company.com/example/project |
| TRACKER      | Url of the base issue tracker                                                                            | https://jira.internal.company.com                |
| BUILD_SERVER | Url of the base build server which started this security test                                            | https://jenkins.internal.company.com             |
| SCM_SERVER   | Url of the base source code managment server on which the source code is stored                          | https://git.internal.company.com                 |
