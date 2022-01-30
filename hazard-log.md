| Hazard number  |                                        Hazard description                                       |            Potential Clinical impact            |                 Possible causes                  |         Existing controls          | Initial Severity               |    Initial Likelihoos        | Intial Risk  |                                                                                                                                                      Design controls                                                                                                                                                         |                                                       Test controls                                                           |                                                  Training Contrpl                                           | Business Process Change   | Residual Severity                |     Residual Likelihood        |  Residual Risk            |                                                   Actions                                                   |              Owner         | Hazard Status |
|----------------|-------------------------------------------------------------------------------------------------|-------------------------------------------------|--------------------------------------------------|------------------------------------|--------------------------------|------------------------------|--------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|---------------------------|----------------------------------|--------------------------------|---------------------------|-------------------------------------------------------------------------------------------------------------|----------------------------|---------------|
|                |                                                                                                 |                                                 |                                                  |                                    |                                |                              |              |                                                                                                                                                                                                                                                                                                                              |                                                                                                                               |                                                                                                             |                           |                                  |                                |                           |                                                                                                             |                            |               |
|        1       |                    Errors could occur during data processing                                    | Misdiagnosis leading to under or overtreatment  |                  Technical error                 |   In built python error messages   |       Considerable             |     Low                      |       2      |                                                                                                              Unit tests, integration tests, error handling and error messages will be built into the tools code                                                                                                              |                                Dummy data of with known movement will be used to test the tool                                |                                                     N/A                                                     |            N/A            |               Considerable       |              Very low          |               2           |                 Tests to be integrated into code to reduce chances of data processing error                 | Haris Shuaib               |    Closed     |
|        2       | Software used within the tool can be updated leading to unknown changes in tools functionality  | Misdiagnosis leading to under or overtreatment  |                   Human error                    | None, introduction of a new system |       Considerable             |    Medium                    |       3      |                                                                          A requirement.txt is used for dicomserver to store required versions of all software used within. Specific versions of the software used for this tool will be added to it.                                                                         |               Testing of new versions of all software used within the tool will be undertaken before deployment               | Instructions for installation using requirements.txt will be made available to those installing dicomserver |            N/A            |               Considerable       |              Very low          |               2           |               Relevant software used for tool to be added to requirements.txt for dicomserver               | Haris Shuaib               |    Closed     |
|        3       |  Alterations to the coding of the tool could lead to unknown changes in the tools functionality | Misdiagnosis leading to under or overtreatment  |                   Human error                    | None, introduction of a new system |       Considerable             |    Medium                    |       3      | All staff altering this code will be required to do so using GitHub. This will maintain version control and audit trails for all changes made to the code.  Independent code review will also be undertaken on all code before deployment.  Limited staff can approve code changes and deploy them to production             |                                                              N/A                                                              |                        Staff can access training online for use of Git and Bitbucket                        | On going use of Bitbucket |               Considerable       |              Very low          |               2           |                       Develop using git in GitHub.                                                          | Haris Shuaib.              |    Closed     |