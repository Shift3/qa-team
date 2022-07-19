# QA Sprint Process
## Project-Under-Test is Prepared
- Website/Application is deployed to a staging environment. 
- Ensure that the site is working as intended before QA starts testing.
- Developer will prepare an Acceptance Test per the Bitwise guidelines.
- Lead Dev will create the Acceptance Test as an issue in Github with:
  - Short project or feature description
  - Delivery / Testing time frame
  - Associated project board
  - Sandbox URL / Testflight App Name
  - App Version number(s) to be tested
  - Devices / Browsers to be tested
  - Testing Steps
     - Acceptance Test in Markdown Format. An Acceptance Test will be necessary for all new projects/features, specifically steps for navigating the project / feature.

Sample of Acceptance Test
https://github.com/Shift3/qa-team/issues/97

## Scheduling QA
1. Project Manager (PM) sends an email to qa@bitwiseindustries.com.
  - Provide the following details:
    - Project and client name
    - Billable to the client?
    - Task description
    - Due date (or estimate of testing time required)
    - Names of PM and lead dev
    - Scope of work
    - List of known issues

2. QA Lead will schedule a kickoff meeting with QA Team, devs and PM.

3. If the project doesn’t have a project board in Github, Lead Dev will create a project board for QA using the following column titles as a guide:
  - Pending
  - Accepted
  - In Progress
  - Ready for Retest
  - Done
  - Rejected




## The Kickoff Meeting
1. PM or Dev will introduce the QA Team to the Project-Under-Test via a demo.
2. If applicable, review for each user type’s abilities and limitations.
3. PM / Dev defines the priorities for testing. 
    - Are there any specific devices we should be looking at?
    - What types of testing will we be doing for this project?
    - Are there any forms of compliance that need to be followed?
{reference} https://github.com/Shift3/qa-team/issues/98
4. Points of contact are identified.
5. Identify any known issues to be ignored or that are outside of scope.
6. QA Team is given write access to the Github repository.
7. Credentials are given to the team via **Zoho Vault**. (BWTC-QA Chamber)
8. If QA is billable to the client, such as for time and materials (T&M) projects, PM will add the QA Team to the Tick project.
9. Add QA to the project’s Slack channel
Discussions should occur constantly within the “Working” issue, tagging people as necessary.
10. A timeline for the QA sprints will be established
We generally ask for up to 2 weeks

## Sprint Planning Meeting
1. QA Team meets to review the application, its purpose and the most important functions of the website.
2. QA Lead sets up project in Proofhub with the following:
- Timeline
- Tasks
- Assignments
- Notes from kickoff meeting
3. QA Lead sets up the following in Github repo:
- Milestone 
- Labels 
4. QA Lead schedules Post-Sprint meeting.

# Testing Process
## QA Testing:

1. If a project board has not been set up by the developer, QA will ask for one to be set up {example} (https://github.com/Shift3/qa-team/projects/9)
2. QA Testers will create a copy of the Acceptance Test to work from.
3. QA will generate new issues for discovered problems. Issues will be:
a. Labeled with the QA Sprint, Bug, Defect, Enhancement, etc.
b. Assigned to relevant milestone and project board
c. Assigned to Point of Contact (POC)

## QA Re-Testing:
***If there are multiple issues, please wait until they are all fixed before requesting QA to retest them.***
1. When issues are ready for retest and deployed to a new test version, please label the issues “Ready for Retest”  
- Contact QA through the project’s Slack channel.
2. If the test is successful, QA Tester adds the “Testing Passed” label to the issue, and adds a comment to update the issue.
3. If the testing failed, QA will add feedback on the issue and add the “Testing Failed” label.
- When “Testing Failed”, the retest process restarts.

## Closing Issues:
The dev team is responsible for closing any issues.

## Contact Us:
Please keep in contact with us in the project's Slack channel whenever a push or change is being made on the staging server
For the following, contact QA via the project’s Slack channel
Pushing Updates
Re-testing
All other communication can be done via the issue’s comments section


## Post-Sprint Meeting
1. QA Lead will go over the testing QA has gone through.
2. QA Lead will note some of the issues we ran into and ask the developers questions relevant to those issues.
3. Recommendation for additional sprint or case by case retest will be made based upon workload QA will discuss w/ PM/Devs the duration of the Retesting Sprint


## After the Post-Sprint Meeting
1. QA Lead will close the sprint milestone to mark the end of the sprint.
2. QA Lead will send a Certificate of Completion to the PM and lead dev. This certificate will include:
Types of testing QA has completed
Google Lighthouse score
List of key issues QA has found
Recommendation for additional sprint or case by case retest
3. Close Proofhub.


