BugTracker Requirements

* BugTracker should have authentication and authorization capabilities.
* BugTracker should have user categories such as developer, tester, and project manager.
* BugTracker should allow the users to create, read, update, and delete PRs.
* Problem Report Specification
  * Allow the reporter to choose the bug severity.
  * Allow the reporter to assign it to someone.
  * Allow the reporter to input large text to describe the issue.
* CRUD bug tickets.
  * Bug ticket editor. Allow the bug creator to set the bug's severity, describe the issue, and allow them to assign the bug to someone.
* A bug should be tied to a project.
* Track changes to ticket – Ticket history
* Create tickets through emails
* Reply tickets  and send notifications through emails.
* A bug may have a status.
* Send notifications for new projects or bugs.
* Allow a user to subscribe to get emails for changes in a project or bugs.
* The time a bug was reported, its severity, the erroneous program behavior, and details on how to reproduce the bug, as well as the identity of the person who reported it, and any programmers who may be working on fixing it.
* Allow the user to set bug similarity level: duplicate or related to a different 

Problem Report Life-cycle
Reference: http://www.no.freebsd.org/doc/en_US.ISO8859-1/articles/pr-guidelines/article.html

* The Reporter submits a bug report on the website. The bug is in the Needs Triage state.
* A developer1 confirms that the bug report has sufficient information to be reproducible. If not, they need to go back and forth with the reporter to obtain the needed information. At this point the bug is set to the Open state.
* Developer2 takes interest in the PR and assigns it to themself, or developer1 decides that developer2 is best suited to handle it and assigns it to them. The bug should be set to the In Discussion state.
* Developer2 has a brief exchange with the reporter/originator (making sure it all goes into the audit trail) and determines the cause of the problem.
* Developer2 creates a patch for the bug and fixes the problem, and submits it in a follow-up, asking the reporter/originator to test it. They then set the PR's state to Patch Ready.
* A couple of iterations later, both developer2 and the originator are satisfied with the patch, and developer2 commits it to current or stable branch, making sure to reference the PR in his commit log (and credit the originator if they submitted all or part of the patch) and, if appropriate, start an MFC countdown. The bug is set to the Needs MFC state. MFC (Merge From Current).
* If the patch does not need MFCing, developer2 then closes the PR as Issue Resolved.

Note: Many PRs are submitted with very little information about the problem, and some are either very complex to solve, or just scratch the surface of a larger problem; in these cases, it is very important to obtain all the necessary information needed to solve the problem. If the problem contained within cannot be solved, or has occurred again, it is necessary to re-open the PR.
