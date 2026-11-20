# Research and Supporting Evidence

## Overview
While making this repository I have conducted research to better understand the benefits and risks created by AI-assistance in software development. AI tools have made abundant leaps in capability when it comes to generating code and general debugging. However as these tools are being given larger and larger roles it becomes even more important to understand how using these tools affects software quality and security. 

My research is going to serve as the foundation for the guidelines and workflow presented throughout this repository. The goal is not to argue for or against the use of AI when writing code, but to identify areas of the software developmoent cycle where AI usage can excel and where human involvement is still integral and should be required. 

---

## 1. Security Risks of AI-Assisted Code

**Source:** Perry, N., Srivastava, M., Kumar, D., & Boneh, D. (2023). *Do Users Write More Insecure Code with AI Assistants?*

[Read the research paper](https://doi.org/10.1145/3576915.3623157)

### Key Findings

In this study, the researchers compared programmers who were assigned with security related programming tasks, one group with AI assistance and one group without. 


They found that participants using an AI coding assistant generally produced less secure code than participants without AI assistance. Interestingly, participants using AI were also more likely to believe that the code they produced was secure.

This suggests that AI tools can introduce security risks while also increasing the confidence that developers have in their solutions.

### Limitations

The study focused on security-related tasks and used an earlier version of an AI coding assistant. Its findings do not establish that all AI-generated code is insecure or that newer tools perform identically.

### Application to This Project

This study supports my argument that developers should not automatically trust AI-generated code simply because it looks correct.

I plan to use this research to support recommendations involving independent code review, security checks, and verifying AI-generated implementations before merging them into shared projects.

---

## 2. Developer Understanding and AI-Generated Code

**Source:** Vaithilingam, P., Zhang, T., & Glassman, E. L. (2022). *Expectation vs. Experience: Evaluating the Usability of Code Generation Tools Powered by Large Language Models.*

[Read the study](https://ml4code.github.io/publications/vaithilingam2022expectation/)

### Key Findings

Researchers observed 24 participants using GitHub Copilot to complete programming tasks.

Although participants generally appreciated Copilot and found its suggestions useful, many struggled to understand, modify, and debug the code it generated.

The study also found that Copilot did not consistently improve task completion times or success rates.

These findings suggest that generating code quickly does not always make the overall development process easier.

### Limitations

The study involved a relatively small group of participants and an earlier version of GitHub Copilot. The results may not represent the capabilities of newer AI coding tools.

### Application to This Project

This study directly relates to one of my main concerns: developers becoming too dependent on AI-generated solutions without understanding how they work.

I plan to use this research to support the **Understand Before You Merge** principle.

Developers should be able to explain how their code works, why an implementation was chosen, and how it fits into the larger project before submitting or approving it.

---

## 3. Productivity Benefits of AI Coding Tools

**Source:** Peng, S., Kalliamvakou, E., Cihon, P., & Demirer, M. (2023). *The Impact of AI on Developer Productivity: Evidence from GitHub Copilot.*

[Read the research paper](https://arxiv.org/abs/2302.06590)

### Key Findings

Researchers conducted a controlled experiment examining how GitHub Copilot affected developer productivity.

Participants were asked to implement an HTTP server using JavaScript. The group using GitHub Copilot completed the task approximately **55.8% faster** than the group without AI assistance.

This provides evidence that AI coding tools can significantly improve productivity for certain programming tasks.

### Limitations

The experiment focused on a specific programming task rather than long-term development in a large existing codebase.

The results should not be interpreted as evidence that AI improves productivity by the same amount for every developer or software project.

### Application to This Project

This research helps demonstrate why AI coding tools can be valuable resources for software developers.

My goal is not to discourage AI usage, but to promote responsible practices that allow developers to take advantage of productivity improvements without sacrificing code quality or understanding.

I plan to reference this research when discussing appropriate uses of AI coding tools, such as generating initial implementations and assisting with repetitive programming tasks.

---

## 4. Limitations of AI-Assisted Developer Productivity

**Source:** Becker, J., Rush, N., Barnes, B., & Rein, D. (2025). *Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity.* METR.

[Read the original study](https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/)

[Read the February 2026 research update](https://metr.org/blog/2026-02-24-uplift-update/)

### Key Findings

METR conducted a study involving 16 experienced developers working on 246 tasks in open-source projects they were already familiar with.

Surprisingly, the researchers found that developers using AI assistance took approximately **19% longer** to complete their tasks compared with developers working without AI.

Developers also tended to overestimate how much AI improved their productivity.

However, METR published an update in February 2026 suggesting that newer AI tools were likely providing greater productivity benefits. The researchers explained that selection biases in their newer experiment made it difficult to determine the actual size of those improvements.

### Limitations

The original study focused on experienced developers working in familiar codebases using AI tools available in early 2025.

These results do not mean that AI always makes developers slower. The findings are also becoming less representative as AI coding tools continue to improve.

### Application to This Project

This research demonstrates that developers should not assume AI is automatically the fastest or most effective approach to every programming task.

I want my guidelines to encourage developers to consider whether AI assistance is appropriate for a particular situation.

For example, AI might be useful for generating repetitive code or exploring an unfamiliar library, but it may be less helpful when making complicated changes to an existing system that requires substantial context.

Developers should evaluate the usefulness of AI rather than relying on it for every task.

---

## 5. Secure Software Development Standards

**Source:** Souppaya, M., Scarfone, K., & Dodson, D. (2022). *Secure Software Development Framework (SSDF) Version 1.1: Recommendations for Mitigating the Risk of Software Vulnerabilities.* National Institute of Standards and Technology.

[Read the NIST framework](https://csrc.nist.gov/pubs/sp/800/218/final)

### Key Findings

The National Institute of Standards and Technology developed the Secure Software Development Framework to provide recommendations for reducing security vulnerabilities throughout the software development lifecycle.

The framework emphasizes secure development practices, identifying vulnerabilities, and verifying software before release.

Although this framework was not specifically designed for AI-assisted software development, many of its recommendations remain relevant when AI tools are used to generate or modify code.

### Limitations

The framework is designed for a broad range of software development organizations rather than specifically for student development teams.

Some practices may require additional resources or formal processes that are not practical for small educational projects.

### Application to This Project

I plan to use this framework as a foundation for the security and verification portions of my guidelines.

However, I want to adapt these practices to my actual audience of UCSB Computer Science students.

Rather than requiring complicated professional security procedures, my guidelines will focus on realistic practices such as checking user input, protecting sensitive information, reviewing changes, and testing important functionality before merging code.

---

## Overall Research Findings

After reviewing these sources, I identified several important ideas that will guide the development of this repository.

First, AI coding tools can improve developer productivity, but those improvements depend on the task, the developer, and the surrounding development environment.

Second, AI-generated code can introduce security vulnerabilities and other problems that may not be immediately obvious. This makes independent verification and code review especially important.

Third, generating working code is not the same as fully understanding it. Developers still need to understand their implementations and be able to explain their decisions to other members of their team.

Finally, established software development practices such as code review, testing, and security verification remain relevant even as AI tools become more capable.

## How This Research Influences the Guidelines

| Research Finding | Guideline or Workflow Recommendation |
|---|---|
| AI assistance can introduce security vulnerabilities. | Independently review AI-generated code for security concerns. |
| Developers may struggle to understand generated solutions. | Require developers to explain their implementations before merging. |
| AI can improve productivity on certain tasks. | Encourage AI assistance when it provides a practical benefit. |
| AI does not consistently improve productivity in every environment. | Evaluate when using AI is actually appropriate. |
| Secure development requires verification throughout the process. | Include human review, testing, and security checks in the development workflow. |

## Conclusion

The research reviewed throughout this document reinforces the main argument of this project: AI-assisted software development can be beneficial, but developers must remain responsible for the code they produce.

AI tools should be used to support software development rather than replace the judgment and technical understanding of human developers.

The guidelines and workflow included in this repository are designed to help developers balance the benefits of AI assistance with the responsibilities that come with writing and maintaining software.