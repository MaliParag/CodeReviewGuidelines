# Code Review Core Guidelines
Author: Parag Mali

# 1. Title

#### 1.1 Be concise
The title of the pull request should be descriptive enough to give a clear idea about the changes made, while also being concise enough to fit in a single line.

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
Add a delimited text in pascal case in the title to higlight the affected area. By adding a prefix to the pull request title makes it easier to search for (in an email client and pull request portal) and filter pull requests based on their type. This can be especially helpful in large projects where there are many pull requests. A clear and consistent prefix makes it easier to understand the purpose of a pull request without having to read the entire title. Do not add multiple prefixes because you may end up with a noisy title.

**Examples**

- [Search] Optimized search algorithm for faster results
- [Payments] Added support for new payment gateway
- [Authentication] Implemented two-factor authentication for added security

#### 1.4 Tag pull requests
Use tagging feature in your project management tool to tag your pull requests. When you add these tags to your pull request they usually autocomplete resulting no typos as compared to prefix in the title. Same tags can be added to the work items related to the pull request. It makes it easier to search for all work-items and pull requests using one query in the project management tool. The reason we need both prefix and tags is that tags generally do not show up in the email notifications you receive related to pull requests. Another advantage of tags is that you can tag your pull request with multiple tags. Adding multiple prefixes in the title will only introduce noise.

### Enforcement 
To enforce these guidelines, code reviewers can check the pull request titles and provide feedback to the submitter if necessary. Teams can also use automated tools to check if pull request titles meet the requirements.

### Exceptions
There may be situations where the changes being made are difficult to describe in a concise title, or where a generic title is sufficient. In such cases, it is important to ensure that the description of the pull request provides enough information about the changes.


# 2. Description  

#### 2.1 Write documentation for future
Pull request description is documentation for future. Write it in a way that assumes that reader has no context of this change.

#### 2.2 Include links to other related pull requests, documents, changes etc.
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



# Review

#### Author is a first reviewer
Make sure you review you own pull request. Add comments to your own pull request where changes should be made. Make all required changes before adding other reviewers.

#### Add your own team or project alias
Include your own team and project team alias. Include at least one senior reviewer from your team.

#### Add affected area owners
Make sure you find out who owns the area that is affected by your changes and include all affected area owners. Include their team alias and at least one senior member of the team individually per affected area.

#### Add a programming language expert
Make sure at least one reviewer in the list of reviewers is programming language expert. If not, find out who can help and include them as a reviewer.

### Enforcement

### Exceptions

# Check-in

#### Get sign-off from all stakeholders

#### Get sign-off on latest iteration from at least one reviewer 

#### Make sure build succedes

#### Squash commits and merge as a single commit

#### Complete related work items

### Enforcement

### Exceptions

# Ettiquetts

# Linking work items
## Quality of work items
## Bugs
## Iteration
## Marking it complete

# Title
## Text tags
## Email search
## Automated tags

# Description
## documentation
## Why
### documents, links, other prs
## Changes
## Testing
### Screenshot
### Command line 
### Testing steps

# Code reviewers
## Seniors
## Owners
## Language experts
## Immediate team or v-team
## Required and optional reviewers

# Publishing the PR
## Draft PR
## Abandoning PR

# Review
## Time
## optional comments
## Required comments
## Kudos and nits
## gifs - lighthearted
## @mention
## citing necessary guidelines
# Merge or Abandon

# Blocking the PR
# Approving the PR
# Approving with suggestions
# Rejecting to review
# Declining the PR

## Work in progress
## Explicitly @mention


## Merging the pull request
### Squash commit

# Selecting the branch to commit
## On demand build branch
## Validation branch
## Bugfix branch
## Dev branch
## Mainline

# Description

## 1: Do make the pull request easy to review.

#### 1.1: Do break up larger changes into smaller, manageable chunks.

eiter pull request or commits

#### 1.2: Do use clear and concise commit messages.
#### 1.3: Do avoid unrelated changes in the same pull request.

Single Responsibility Principle

#### 1.4: Do write a clear description of what the changes do and why they are necessary.

#### 1.5: Do mention any related issues or pull requests in the description.

#### Enforcement
Enforcing this guideline can be achieved through code reviews that ensure that each pull request is focused on a single task or issue. Pull request authors can help enforce this guideline by breaking up changes into smaller, more manageable pieces.

#### Exceptions
In some cases, it may be necessary to make multiple changes in a single pull request. For example, if the changes are all related to the same feature or issue, it may make sense to include them in the same pull request.

#### Responsibilities
The pull request author is responsible for ensuring that the changes are easy to review. The reviewer is responsible for verifying that the changes are well-organized and focused.

## 8: Follow established coding standards.

#### Follow established coding standards.
#### Follow best practices for the programming language and framework being used.
#### Follow established conventions for naming, formatting, and documentation.

#### Enforcement
Code reviews can help enforce adherence to coding standards. Automated tools can also help identify issues with naming, formatting, and documentation.

#### Exceptions
In some cases, it may be necessary to deviate from established coding standards. In these cases, the pull request author should clearly explain the reasons for the deviation.

#### Responsibilities
The pull request author is responsible for following established coding standards. The reviewer is responsible for verifying adherence to coding standards. The team lead or project manager is responsible for establishing and communicating coding standards.

## 4: Write clear, readable code.

#### Use clear and descriptive variable names.
#### Use consistent formatting and style.
#### Use comments to explain complex or non-obvious code.

#### Enforcement
Automated tools can help enforce consistent formatting and style. Code reviews can help enforce the use of clear variable names and comments.

#### Exceptions
In some cases, it may be difficult to come up with descriptive variable names or to write clear comments. In these cases, the pull request author should strive to make the code as readable as possible.

#### Responsibilities
The pull request author is responsible for writing clear, readable code. The reviewer is responsible for verifying that the code is clear and easy to read.


## 2: Avoid unnecessary changes.

#### Avoid making changes that are unrelated to the task at hand.
#### Avoid changing formatting or whitespace unless necessary.
#### Avoid adding debugging code or commented-out code.

#### Enforcement
Code reviews can help enforce this guideline by identifying changes that are unrelated to the task at hand. Pull request authors can help enforce this guideline by only making necessary changes.

#### Exceptions
Sometimes, seemingly unrelated changes may be necessary to complete the task at hand. For example, a change to a shared library may require updates to several projects that depend on that library.

#### Responsibilities
The pull request author is responsible for ensuring that changes are related to the task at hand. The reviewer is responsible for identifying any unnecessary changes.


## 3: Consider the impact of changes on other code.

#### Consider the impact of changes on other parts of the codebase.
#### Consider the performance implications of changes.
#### Consider the compatibility of changes with existing code.

#### Enforcement
Code reviews can help enforce this guideline by identifying potential issues with changes. Pull request authors can help enforce this guideline by carefully considering the impact of their changes before submitting a pull request.

#### Exceptions
In some cases, changes may need to be made even if they have negative implications for performance or compatibility. In these cases, the pull request author should clearly explain the reasons for the changes and provide any necessary documentation.

#### Responsibilities
The pull request author is responsible for considering the impact of their changes. The reviewer is responsible for verifying that potential issues have been considered.

## 5: Test code thoroughly.

#### Don't submit code that hasn't been tested.
#### Don't submit code that introduces new bugs.
#### Don't submit code that breaks existing tests.
#### Do test all new and modified functionality.
#### Do test edge cases and error handling.
#### Do test on multiple platforms and configurations.

#### Enforcement
Automated testing can help enforce this guideline by catching bugs before they are introduced into the codebase. Code reviews can also help identify potential issues and areas where additional testing may be necessary.

#### Exceptions
In some cases, thorough testing may not be possible or practical. In some cases, bugs may be introduced despite best efforts to prevent them. In these cases, the pull request author should work quickly to fix the issue and communicate with the team.

#### Responsibilities
The pull request author is responsible for thoroughly testing their code and ensuring that it does not introduce new bugs. The reviewer is responsible for verifying that the code has been adequately tested and does not introduce new issues.

## 6: Document changes.

#### Document new or modified functionality.
#### Document any new or modified APIs.
#### Document any changes to configuration or deployment processes.

#### Enforcement
Code reviews can help enforce this guideline by ensuring that changes are properly documented. Pull request authors can help enforce this guideline by providing clear documentation along with their changes.

#### Exceptions
In some cases, it may be difficult to document every aspect of a change. In these cases, the pull request author should strive to document the most important aspects of the change.

#### Responsibilities
The pull request author is responsible for documenting changes. The reviewer is responsible for verifying that changes have been adequately documented.

## 7: Be respectful and professional.

#### Be respectful and professional in all communications.
#### Be open to feedback and constructive criticism.
#### Be willing to collaborate with others.

#### Enforcement
The team lead or project manager can help enforce this guideline by setting expectations for respectful and professional behavior. Team members can help enforce this guideline by modeling respectful and professional behavior in their own interactions.

#### Exceptions
There are no exceptions to this guideline. Respectful and professional behavior is always expected.

#### Responsibilities
All team members are responsible for maintaining a respectful and professional environment. Team leads or project managers are responsible for addressing any behavior that violates this guideline.

## Guideline 10: Communicate effectively.

#### Communicate clearly and effectively in all interactions.
#### Communicate changes to the team and stakeholders.
#### Communicate any issues or blockers that may affect progress.

#### Enforcement
The team lead or project manager can help enforce this guideline by setting expectations for clear and effective communication. Team members can help enforce this guideline by providing regular updates on their progress and any issues they encounter.

#### Exceptions
There are no exceptions to this guideline. Effective communication is essential for successful collaboration.

#### Responsibilities
All team members are responsible for communicating effectively. The team lead or project manager is responsible for ensuring that effective communication is taking place and addressing any issues that arise.




