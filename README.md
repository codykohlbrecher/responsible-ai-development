# Responsible AI-Assisted Software Development

This repository provides a practical guide for using AI coding tools responsibly while being able to maintain software quality, developer understanding, and human accountability.

## About This Project

In the software industry Artificial intelligence tools are being more and more frequently. Agentic AI coding tools like ChatGPT, Codex, and Copilot  help developers generated tests, write, and debug code. These tools can improve productivity, however they also introduce risks when developers begin over-relying on solutions written by AI without fully understanding the intricacies of how they work.

This repository is being written for my WRIT 105AI final project. The main purpose of this is to provide practical guidlines and a simple workflow for new developers to responsibly use AI assistance when developing or reviewing software.  

This project is designed primarily for UCSB Computer Science students who are developing software in a team setting. My intended audience is for students who are working on the legacy code base project in CMPSC 156, Advanced App Programing. However the guidlines and workflow included in this repo is intended to be useful for any junior developers or engineers who are new to using AI tools in their development workflow. 

## The Problem
The biggest problem that I have encountered and witnessed while developing software begins when developers blindy trust AI-generated code since it passes automated testing.

Even when AI tools generate code that is functionally correct, it is possible that the code is inefficient, produces vulnerabilities, and or is not scalable to the overall goals of the project. 

Even when AI-generated code has passed all of your testing it should not be assumed that the code is efficient, secure, and has met the standard of quality you should expect when writing quality software. 

**Developers should never merge code that they can not UNDERSTAND, EXPLAIN, and DEFEND, regaurdless of whether AI assistance was used in development**

AI should act as a tool to assist developers in solving problems and should never replace their responsibility to understand the solutions.

## Project Goals


1. Establish practical guidelines for using AI coding tools responsibly.

2. Discourage blindly accepting AI-generated code while encouraging critical evaluation of all AI-generated parts of their project.

3. Promote human oversight throughout all aspects of the software development process.

4. Provide a practical and repeatable workflow for generating, testing, and reviewing AI-assisted code.

5. Place an emphasis on accountability, collaboration, and transparency in team-based software development.

## Core Principles

### 1. Human Accountability

Developers take on sole responsibility for all of the code that they submit or merge. AI tools are not able to take any amount of responsibility regaurdless of their role in the development process. Any bugs or vulnerabilities that are introduced into the code by AI tools must be found and fixed by human developers.


### 2. Understand Before You Merge

It is integral that developers are able to explain how every part of their code works and why that specific implementation was chosen. They should also be able to explain how the new code fits in the existing code base or project. 

If you are not able to explain a solution that an AI tool generated for you then you should review the code more thuroughly before submitting or approving it. 

### 3. Tests Are Necessary, but Not Sufficient

Automated tests are an important part of software development, but passing every test is not a sufficient indicator that your code is correct, secure, or maintainable.

Developers should review the underlying implementation and consider edge cases, security concerns, and alternative approaches.

### 4. Transparency in AI Usage

When working on collaborative projects, developers should document what parts of the project AI tools were used and how. This will allow other members of the team to understand a developers workflow and know which parts of the project require intense review. 

### 5. AI as an Assistant, Not a Replacement



AI coding tools should support learning and problem-solving rather than replace independent thinking. Developers should use AI to improve their understanding of software development, not avoid developing that understanding themselves.

## How to Use This Repository

This repository contains guidelines, checklists, examples, and research intended to help developers establish a responsible AI-assisted development workflow.

| Section | Description |
|---|---|
| [Responsible AI Guidelines](guidelines/responsible-ai-guidelines.md) | Practical recommendations for using AI throughout software development. |
| [Code Review Checklist](guidelines/code-review-checklist.md) | A checklist for evaluating AI-assisted code before approving or merging it. |
| [Human-in-the-Loop Workflow](workflow/human-in-the-loop-workflow.md) | A step-by-step process for using AI while maintaining human oversight. |
| [Example Code Review](workflow/example-code-review.md) | An example demonstrating how the guidelines can be applied. |
| [Research and Sources](research/sources-and-findings.md) | Research supporting the project's recommendations. |
| [Workshop Feedback](feedback/workshop-feedback.md) | Feedback and revisions collected from student developers. |
| [Development Process](process/process-log.md) | Documentation of how AI and human judgment contributed to this project. |

### Recommended Workflow

**Understand the task → Use AI assistance → Review the generated code → Test and verify → Submit a pull request → Conduct human review → Merge**

The main goal of this specfic workflow is to maintain human judgement throughout each part of the development process. 

## Research and Supporting Evidence

The recommendations that are presented throughout this repository are based on research regaurding AI-assistance in software development, computer security, productivity, and human oversight. 

Instead of operating with the assumption that all AI-generated code is reliable or unreliable, I want to focus on identifying which parts of the development process AI tools can thrive in and which ones need intense human oversight or involvement in. 

A detailed discussion of research findings and supporting sources is available in [Research and Sources](research/sources-and-findings.md).

## Feedback and Future Improvements

These guidelines are intended to be tested and improved through feedback fromn fellow student developers.

As part of this project, I will to share the repository with members of my CMPSC 156 development team and collect feedback regaurding if these recommendations were practical and benneficial to their developement process.

This feedback will help identify which guidelines are realistic for student projects and which may require further revision.

## Final Takeaway
AI coding tools have been proven to be a valuable resource in software development and do not seem to be going anywhere, anytime soon. However it is important to use them responsibly to take advantage of all the the upsides and avoid risk. 


**If you cannot understand, explain, and take responsibility for the code, you should not merge it.**

My goal is not to discourage AI-assisted software development, but to make sure actual human developers remain an active, important participant the developer cycle# responsible-ai-development
This repository covers guidelines and work-flows for responsible AI-assisted software development. These guidelines are going to place an emphasis on  code review, human responsibility, and understanding. 
