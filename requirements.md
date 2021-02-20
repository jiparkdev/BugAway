BugAway Requirements

* BugAway should have authentication and authorization capabilities.
* BugAway should have user categories such as developer, tester, project manager, and system admin.
* BugAway should allow developers, testers, and project managers to create, read, and update PRs.
* BugAway should allow system admins to create, read, update, and delete PRs.
* Problem Report Specification
  * Upon creating a PR, the PR automatically gets the Needs Triage state.
  * When a developer confirms the PR, they can set it to Open state.
  * When a developer gets assigned the PR, then the state is: In Discussion.
  * A developer creates a patch for the bug, then submits it in a follow-up for retest. They set PR state to Patch Ready.
  * After testing, if the issue does not seem to be occurring anymore, assignee can set it to Verified & Fixed.
  * Once a patch has been verified and the issue fixed, then the PR is Marked for Resolution.
  * After the issue is fully resolved, the state changes to "Issue Resolved".
  * All PRs shall be in one of the following states: new, open, in discussion, resolved, closed
  * Allow the reporter to select the issue type: enhancement, question, bug, feature request, discussion
  * Allow the reporter or assignee to select the issue resolution: unsolved, wontfix, stale, duplicate, backlog, needs more information.
  * Allow the reporter or assignee to set the PR state to: open,
  * Allow the reporter to input a title of the issue.
  * Allow the reporter to input large text to describe the issue.
  * Allow the reporter to choose the severity of the issue.
  * Allow the reporter to assign the PR to one person, CC to multiple, or to no one.
  * Allow the reporter to choose a project for which the bug is under.
* Track changes to ticket – ticket history
* Reply tickets  and send notifications through emails.
* Send notifications for new projects or bugs.
* Allow a user to subscribe to get emails for changes in a project or bugs.

Problem Report Life-cycle
Reference: http://www.no.freebsd.org/doc/en_US.ISO8859-1/articles/pr-guidelines/article.html
