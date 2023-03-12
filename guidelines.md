# Code Review Core Guidelines
Author: Parag Mali

# 1. Title

#### 1.1 Be concise
The title should be descriptive enough to give a clear idea about the changes made, while also being concise enough to fit in a single line.

#### 1.2 Use action oriented language
Use action-oriented language that accurately describes the changes being made. This helps reviewers to understand what the code does and why it was changed.

**Examples**

- "Added new feature for user authentication"
- "Fixed issue with database connection"
- "Refactored code for better readability"
- "Implemented error handling for edge cases"
- "Optimized performance by reducing database queries"
- "Added input validation for user inputs"
- "Resolved conflicts with merge of upstream changes"
- "Improved UX by adding pagination for search results"
- "Added support for multiple languages"
- "Created API endpoint for user profile information"

#### 1.3 Use a prefix to highlight modified area
Add a delimited text in pascal case in the title to higlight the affected area. By adding a prefix to the title makes it easier to search for (in an email client and project management portal) and filter based on their type. This can be especially helpful in large projects where there are many code changes. A clear and consistent prefix makes it easier to understand the purpose of a change without having to read the entire title. 

Do not add multiple prefixes because you may end up with a noisy title.

**Examples**

- [Search] Optimized search algorithm for faster results
- [Payments] Added support for new payment gateway
- [Authentication] Implemented two-factor authentication for added security

#### 1.4 Tag pull requests
Use tagging feature in your project management tool to tag your changes. These tags usually autocomplete resulting in reduced number of typos as compared to prefix in the title. Same tags can be added to the related work-items like tasks and bugs. It makes it easier to search for all work-items and changes using one query in the project management tool. The reason we need both prefix and tags is that tags generally do not show up in the email notifications you receive related to the code changes. Another advantage of tags is that you can tag your code changes with multiple tags. Adding multiple prefixes in the title will only introduce noise.

### Enforcement 
To enforce these guidelines, code reviewers can check the pull request titles and provide feedback to the submitter if necessary. Teams can also use automated tools to check if pull request titles meet the requirements.

### Exceptions
There may be situations where the changes being made are difficult to describe in a concise title, or where a generic title is sufficient. In such cases, it is important to ensure that the description of the pull request provides enough information about the changes.


# 2. Description  

#### 2.1 Write documentation for the future
Description is the documentation for the future. While writing description assumes that reader has no context of this change.

#### 2.2 Include links to other related code changes, documents, etc.
Include links to the documents that give additional information related to this pull request, may it be a spec or an one pager. Provide links to other related pull requests. 

#### 2.3 Provide a brief summary of the changes
Start the description with a brief summary of the changes being made. This should be concise and give an overview of what the pull request does.

#### 2.4 Explain the reasoning behind the changes
Provide a detailed explanation of why the changes were made. Mention alternative approaches considered and reasons behind choosing current approach. This can help reviewers understand the context and make more informed decisions about the code changes.

#### 2.5 Use @mention to bring attention any potential issues or areas for further review
Use @mention to mention all stakeholders and to bring their attention to potential impacts of current code changes or areas where you want input from reviewers.

#### 2.6 Include test cases or link to the test case document
Include all test cases with steps that were used to validate the changes. Include commands or scripts used for validation.

#### 2.7 Include screenshots and outputs of the test cases
Include screenshots or outputs of the test cases showing that all test cases passed. Include outputs, so future testers can verify their outputs with your output.

### Enforcement
To enforce these guidelines, reviewers can check the pull request description and provide feedback to the submitter if necessary. Teams can also use automated tools to add an agreed upon template to the description box automatically when a new pull request is created. Reviewers need to make sure all details are provided in the added template.

### Exceptions
There may be situations where the changes being made are minor or self-explanatory, and a detailed description is not necessary. However, it is always better to err on the side of providing more information rather than less, to ensure that reviewers have all the information they need to make informed decisions.

# Adding reviewers

#### Author is a first reviewer
Make sure you review you own pull request. Add comments to your own pull request where changes should be made. Make all required changes before adding other reviewers.

#### Add your own team or project alias
Include your own team and project team alias. Include at least one senior reviewer from your team.

#### Add affected area owners
Make sure you find out who owns the area that is affected by your changes and include all affected area owners. Include their team alias and at least one senior member of the team individually per affected area.

#### Add a programming language expert
Make sure at least one reviewer in the list of reviewers is programming language expert. If not, find out who can help and include them as a reviewer.

#### Indicate if reviewer is a required reviewer or an optional reviewer
While adding reviewers, make sure you indicate who is required and who is not-required to review the changes.

### Enforcement
The team lead or project manager is responsible for establishing and communicating code review policies with the team. Reviewers should add additional reviewers as they may see fit. Author is responsible for getting code reviewed by all required reviewers.

### Exceptions
While code review is an important process to ensure the quality of the codebase, there may be certain situations where getting code reviewed may not be necessary or feasible. If the changes being made are very minor, such as fixing a typo or adjusting formatting, it may not be necessary to have the code reviewed. Sometimes time sensitive changes like build fixes over weekends could be self-approved, even though it is not ideal.

# Publishing the code changes

## Mark code changes as "draft" if they are in progress
If changes are still in progress, but you want early feedback on the design, make sure you mark the changes with prefix like draft or WIP (work in progress). 

## Publish changes only after you thorough validation
After thorough validation is done, publish the code changes. 

# Review

## Author's responsibilites

#### Give sufficient time to reviewers to review the changes
Team lead should provide guidance on review SLA. Author should follow up with reviewers if code hasn't reviewed within SLA.

### Use code review comments as a learning opportunity
Author's should be open to feedback, constructive criticism, and collaborate with others. 

#### Mark comments as Pending, Resolved, Won't Fix, Closed etc.

- Pending: If a comment requires further discussion or clarification before it can be resolved, mark it as Pending. This indicates that the issue has been acknowledged, but further action is required before it can be resolved.

- Resolved: When an issue raised in a comment has been addressed or fixed, mark the comment as Resolved. This indicates that the issue has been resolved and no further action is required.

- Won't fix: If an issue raised in a comment is not a critical issue or if the proposed solution is not feasible, mark the comment as Won't Fix. This indicates that the issue has been acknowledged, but it will not be addressed at this time.

- Closed: If no further action or discussion is required, mark the comment as Closed.

## Reviewer's responsibilities

#### Review changes within SLA
Decline to review if you won't be able to review within SLA.

#### Use tags like optional and required while adding comments
Make it very clear what comments are optional to fix and what comments should be fixed. Appreciate good work when you like something using "kudos" prefix. Use "nit" prefix when you are nitpicking. 

#### Cite references while adding comments
If the comment is related to coding style cite language specific coding style guidelines. For example, for CPP reviewers could cite guidelines from https://github.com/isocpp/CppCoreGuidelines. If comment is related to engineering practice, cite appropriate documents and provide links to the documents. 

#### Avoid generic comments
Avoid generic comments like "fix this", "bug here". Explain what should be fixed and why there is a bug in the code. 

#### Vote on the code changes after the review

- Approved: Use the "Approved" label when you have thoroughly reviewed the changes and believe that they meet the required quality standards. This label indicates that you are satisfied with the changes and that they can be merged into the codebase.

- Approved with suggestions: Use the "Approved with suggestions" label when you believe that the changes are generally good, but there are minor issues or suggestions that should be addressed before the changes are merged. This label indicates that you are satisfied with the changes but there are some additional improvements that could be made.

- Rejected: Use the "Rejected" label when you believe that the changes are not up to the required quality standards or that they introduce issues or bugs into the codebase. This label indicates that the changes need significant work before they can be merged.

- Blocked: Use the "Blocked" label when you have raised an issue or question in the pull request and are waiting for the author to provide more information or make changes. This label indicates that you are unable to approve or reject the changes until further action is taken.

## Common responsibilities

#### Be respectful and professional in all communications.
#### Make sure all agreed upon guidelines are followed.

# Check-in

#### Get sign-off from all reviewers
Make sure all required reviewers have signed off on the code changes.

#### Get sign-off on latest iteration from at least one reviewer 
If you need to push code changes after last reviwer has signed-off make sure you get additional approval on the latest iteration of changes.

#### Make sure build succeedes with latest iteration of code changes
Build changes locally or on a build machine before check-in. Make sure your changes do not break builds of any other projects.  

#### Squash commits and merge as a single commit
Squash all commits and merge the changes to mainline as a single commit.

#### Select appropriate target branch 
Make sure the selected target branch for check-in is the correct branch. 

#### Complete related work items
Once code changes are checked-in, mark the appropriate work-items as completed.

#### Delete remote-branch and local-branch
If you have remote and local branch related to checked-in code changes, you may delete those branches.

# Code changes

#### 1.1: Do break up larger changes into smaller, manageable chunks.
#### 1.2: Do use clear and concise commit messages.
#### 1.3: Do avoid unrelated changes in the same pull request.
#### Follow established coding standards.
#### Follow best practices for the programming language and framework being used.
#### Follow established conventions for naming, formatting, and documentation.
#### Use comments to explain complex or non-obvious code.
## 2: Avoid unnecessary changes.
#### Avoid making changes that are unrelated to the task at hand.
#### Avoid changing formatting or whitespace unless necessary.
#### Avoid adding debugging code or commented-out code.

