[![Stories in Ready](https://badge.waffle.io/unicef/etools-issues.png?label=ready&title=Ready)](https://waffle.io/unicef/etools-issues)
# etools-issues
This repository is central to all issue tracking in the eTools project. It is integrated to [Waffle](https://waffle.io/unicef/etools-issues) - the eTools team's issue management tool. 
All issues logged in [Waffle](https://waffle.io/unicef/etools-issues) are readily available in this repository. Any updates done to the issue in GitHub is reflected in Waffle and vice versa. 

[issues-only](https://help.github.com/articles/creating-an-issues-only-repository/) repository for eTools project

### Prerequisites

You need a GitHub account to access the [etools-issues](https://github.com/unicef/etools-issues) repository. 

This is the [Waffle](https://waffle.io/unicef/etools-issues) board to view all the issues by current status. 

## Getting Started

Remember to request access to the [etools-issues](https://github.com/unicef/etools-issues) repository so that you can start working/adding/editing the issues in Waffle/GitHub. 

Access will be provided by GitHub [UNICEF](https://github.com/orgs/unicef/people?page=2) admin. 





### Target Audience

This is a step by step instruction manual for all developers who will work on the issues raised in Waffle/GitHub. 


### Roles and Responsibilities

	Product team members/Engineering team members can log/create issues in Waffle.

	All new issues are created in the Inbox column. 

	Based on urgency and priority the product team will move issues to the Backlog column.

	The Engineering team lead will review the Backlog column and move issues/tasks that can be worked on immediately to the On Deck column.

	The team lead can assign issues/tasks from the On Deck to relevant team members or the team member can assign tasks to himself based on understanding of the requirement and available bandwidth


## What are the features of the Waffle Board?

Waffle is a project management tool powered by your GitHub Issues and Pull Requests.
Waffle is built on top of the GitHub API so all the work in GitHub and its status in Waffle remains up-to-date. Status updates are possible from both GitHub and Waffle. 
Waffle also integrates with Slack- so status updates are pushed to relevant Slack channels. 




### The natural progression for an issue

[Recommended workflow for Waffle issues](https://help.waffle.io/automatic-work-tracking/auto-work-tracking-basics/recommended-workflow-using-pull-requests-automatic-work-tracking)



## Example

To move issue#140 from On Deck to In Progress, we created a PR and included the following text in the description
```
 connects unicef/etools-issues#140-test
```



### Moving a card from In Progress to Needs Review

1.	The issue has to already be in the In Progress column 
2.	The issue must have a PR attached to it
3.  The Needs Review column has to be set up for New Collaborator PRs going to it    (Project Settings->Columns)

If all of the above is true, you can use [GitHub Closing Keywords](https://help.waffle.io/faq/waffle-workflow/use-github-closing-keywords-to-connect-prs-to-issues) within the PR's description to move the PR + issue to the Needs Review column.


## Example 
This is the sample text we used in the PR’s description to move the issue from In Progress to Needs Review. 
```
closes unicef/etools-issues#140-test
```
## Moving the issue from Needs Review to Done
To close an issue use [GitHub Closing Keywords](https://help.waffle.io/faq/waffle-workflow/use-github-closing-keywords-to-connect-prs-to-issues) followed by a reference to the issue number in the PR description. This will close the issue once the commit is merged into the default branch. 

## Setting the milestone and size of an issue

## Referencing an issue in an external repository

You can also reference an issue in an outside repository by using username/repo#123. 
If you'd like to add additional information to the branch, you can do so by adding it to the end of the branch name. 
Just separate the repo path and issue number with a "-", or "_", followed by the wording of your choice.

Example of a cross repository issue reference:
```
    username/repo#123-bug-fix
```
In order for a cross repo reference to be picked up, you'll need to have both repos on the same multiple repo board. 
(More info on multi repo boards here)


## Linking two issues together

If you see issues related to each other [do this](https://help.waffle.io/faq/waffle-workflow/can-i-link-two-issues-together) to link them.

## Using GitHub closing keywords to connect PR to issues

Use [GitHub Closing Keywords](https://help.waffle.io/faq/waffle-workflow/use-github-closing-keywords-to-connect-prs-to-issues) to link a PR to an issue. Linking a PR to an issue in this fashion moves the issue to the In Progress column. 


## Using Waffle connect keywords to connect PR to issues 

Use Waffle's connect keywords to connect a PR and an existing issue in such a way that the issue remains open even after the PR is merged with the main branch. It implies that issue is in progress and not yet ready for review. 
(https://help.waffle.io/faq/waffle-workflow/use-waffles-connect-keyword-to-connect-prs-to-issues)

## Keeping PRs and issues separate

If you reference an issue number in your pull request title or description but DO NOT use GitHub's closing keywords or Waffle's "Connect" keywords prior to the issue reference, a separate PR Issue card will be displayed on your Waffle board for that pull request. Likewise, if no issue references are present in the pull request title or description, a separate PR Issue card will be displayed on your Waffle board.

## Closing multiple issues

To close multiple issues, preface each issue reference with one of the above keywords.


For example: 
```
 This closes #34
 ```
 ```
closes #23
```
```
closes example_user/example_repo#42 
```
would close issues #34 and #23 in the same repository, and issue #42 
in the   "example_user/example_repo" repository.



