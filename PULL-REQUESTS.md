# Pull Request Checklist

## Beginning the Work
Good Pull Requests start well before you write your first line of code. Be prepared to craft discreet, focused and intentioned PR's by following a few simple guidelines:

1. Create a __new__ branch
1. Select a branch name that matches your company's guidelines
1. In the absence of guidelines, use a consistent, meaningful branch naming convention. Consider using the story or task identifier in the branch name.
1. Keep the work to a single feature / story / task to limit the scope of the upcoming PR
1. Use meaningful commit messages:
  * Great: `ABC-123: Updated logic to include the correct coefficient multiplier based on the information provided by @teammate in our grooming session on 10/02`
  * Good: `Updated logic to include the correct coefficient multiplier`
  * Poor: `Fixed some things`
  * Bad:  ` `

## Before Submitting a PR
Good code reviews begin with you. Make sure you have done everything possible to ensure that the process goes quickly and that the reviewers have the necessary information to complete the review. Now is the time to take care of the easy things so that the reviewers can focus on the code itself:

1. Make sure the code builds / compiles properly, even if you only made a small change
1. Ensure all Tests in your test suite are passing (if you have a test suite)
1. Make sure all Linter warnings and errors have been addressed
1. If you don't have a Linter, ensure your indentation, spacing and formatting is correct and consistent
1. Make sure you have properly commented your code. If your team uses JSDoc, JavaDoc or something similar, make sure you're compliant
1. Remove all superfluous logging statements (e.g.: `console.log`, `console.warn`, `System.out.println`)
1. Remove all commented-out / hidden code unless including an explanation as to why it is being temporarily hidden
1. If you have copied/pasted code from an online resource, read and review it yourself first. Ensure it meets your standards / requirements.
1. Make sure there are no unnecessary files changed
1. Limit your PR's to a single story and/or ticket
1. Limit the size of your PR's as much as possible

## When Submitting a PR
Aside from writing good, clean code, completing the tasks you're assigned and then running through a "pre-submit checklist", there are some guidelines for how to submit a Pull Request to ensure things go as smoothly as possible:

1. Make sure to highlight dependencies on other branches/projects/versions (e.g.: requires API v2, requires API branch `foo` be merged)
1. If this is a Work-in-Progress (WIP) then tag/label the PR as appropriate
1. Make sure the correct reviewers are included
1. @mention anyone who you specifically want to review/comment on a section
1. Make sure you have left good comments in the PR explaining the changes
1. Make sure there are no Merge Conflicts; address them immediately if they are present
1. Add inline comments in the PR for anything you feel might warrant explanation
1. Expect feedback / changes to come; be open to and receptive of the feedback
1. Immediately review your own PR as if you were the reviewer. Use the checklist below to check your own work before you ask for peer review.

## When Reviewing a PR
Reviewing Pull Requests can be a time consuming process, but it's your opportunity to ensure quality, enforce standards and understand the application you're working on at a deeper level. Set aside time to review code, do it consistently and properly and treat it as important work. There are dozens of things to look for when reviewing code and this is by no means an exhaustive list, but rather a basic guideline to follow for starting the review process:

### General Guidelines
1. Leave positive, helpful feedback
1. Be respectful: Avoid derogatory or condescending words and/or tone
1. Check-out the code and run it in your environment
1. Make sure the code builds / compiles properly
1. Ensure all Tests in your test suite are passing
1. Make sure all Linter warnings and errors have been addressed

### What to Look For
This is not an exhaustive list of every language-specific check you should make, but rather a high-level list of things to review. Your project, codebase, language and tech stack will determine the specific, code-level checks you'll want to make, but here are some simple guidelines:

1. Review the comments: Do they exist? Do they meet your team's requirements?
1. Check for unnecessary logging statements
1. Check for hidden / commented-out code
1. Is there proper error handling in place?
1. Is the complexity level appropriate for the task?
  * Look at the indentation level, is it very deep?
  * Can the code be simplified by creating new functions / classes?
  * etc.
1. Is this code consistent with other, similar parts of the project?
1. Is there similar functionality somewhere else? Can it be reused?
1. Is this using common conventions used elsewhere in the project?
1. Is this code using complex, arcane or shorthand syntax? Has your team agreed to this?
  * Ternary `if`
  * `+,-,!,~` type modifiers
  * Regular Expressions
  * etc.
1. Does the code include Regular Expressions? If so, have you tested them?
1. Is there meta-syntax required, such as Schema.org or another Microformat?
1. Are there accessibility requirements to be considered?
1. Is esoteric knowledge of the project required to understand a feature? If so, are proper comments and / or pointers to documentation made available?

## When Responding to Feedback
When you create a PR, you're asking for someone else's input and you're asking for their time. Be respectful of both and appreciative of any feedback you receive. Try not to take things personally, this is an exercise in nitpicking. Thank the participants for their feedback and approach your fixes / responses with a positive attitude.

1. Keep a positive tone
1. Comment on or address each piece of feedback 
1. Ask for more information if needed
1. Provide clarification if there was a misunderstanding about a feature / decision
1. Try to address the items quickly to reduce the length of the feedback cycle