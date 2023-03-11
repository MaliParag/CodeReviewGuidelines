# Code Review Core Guidelines
Author: Parag Mali

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




