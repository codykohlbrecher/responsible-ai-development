# Code Review Checklist for AI-Assisted Development


## Ground Rule

Each developer on a team is soley responsible for the code they submit whether or not they used AI in its developments. This checklist is designed to help developers maintain this responsibility by developing a proper understanding and properly reviewing code. 

**If you cannot UNDERSTAND, EXPLAIN, and DEFEND your code, you should not merge it.**

## Before Submitting or Approving a Pull Request

### 1. Understanding the Code

- [ ] Can I explain what the code does and why I went with a certain implementation?
- [ ] Have I personally reviewed all changes an agent made?
- [ ] Does this code introduce any new bugs?

### 2. Correctness and Testing

- [ ] Does the implementation address all aspects specified in the original GitHub issue?
- [ ] Have I run the relevant tests and checked the results?
- [ ] Have I considered all possible edge cases or bugs that automated tests could have missed?

### 3. Security

- [ ] Did I check the implementation for potential security vulnerabilities?
- [ ] Are user inputs properly handled and sensitive information protected?
- [ ] Does the code follow the security requirements appropriate for this project?

### 4. Transparency and Team Review

- [ ] Have I explained AI assistance used to generate or modify the code-base?
- [ ] Can other members of my team understand and maintain this implementation?

## Final Check

Before creating or merging any pull requests, it is important that developers understand all of the changes that ahve been made. They should make sure that indipendent verification has occured and the implementation is working as intended. 

If the program passes all automated testing, that is a good sign. But passing alone should never be considered a sufficient measure of whether a PR is ready to be merged. 

At the end of the day the developer and their team are responsible for the final product, not the AI tool that helped generate it.

For more information, see the [Responsible AI Guidelines](responsible-ai-guidelines.md).