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
The study found that participants using an AI coding assistant generally produced less secure code than participants without AI assistance. Interestingly, participants using AI were also more likely to believe that the code they produced was secure. These findings provide evidence that AI tools have the possibility of introducing security risks while also increasing the confidence that developers have in their AI generated solutions.

### Limitations

The study focused on security-related tasks and used early AI models for their expiriments. They were not able to difinitively prove that al AI-generated code is insecure or that the newer, improved models of today also share these issues.  
### Application to This Project

This study supports that developers should not automatically trust the code that AI tools generate simply because they look and seem to be correct. I plan to use my research to support recommendations involving independent code review, security checks, and verifying AI-generated implementations before merging them into shared projects. In CS156 we deal with a lot of web development so it is important to make sure that we are developing a final product that is secure and does not have any major vulnerabilities that could be exploited to access sensetive data. 


---

## 2. Developer Understanding and AI-Generated Code

**Source:** Vaithilingam, P., Zhang, T., & Glassman, E. L. (2022). *Expectation vs. Experience: Evaluating the Usability of Code Generation Tools Powered by Large Language Models.*

[Read the study](https://ml4code.github.io/publications/vaithilingam2022expectation/)

### Key Findings

In this study, researches observed 24 developers who were using GitHub Copilot to complete programming tasks. Participants generally appreciated Copilot and found its suggestions useful. However many of the participants had issues understanding, adding to, and debuging the generated code. They also found that Copilot did not consistently improve task completion times or success rates for every problem. This study adds to the idea that generating code quickly does not always make the overall development process easier.

### Limitations

The study only looked at a relatively small group of participants and an earlier version of GitHub Copilot. The results may not represent the capabilities of the newer AI coding tools that we have today.

### Application to This Project

This study directly relates to one of my main concerns that developers are becoming too dependent on AI-generated solutions without understanding how they work.
I plan to use this research to support the **Understand Before You Merge** principle. It is integral for developers to be able to explain how their code works, why they chose a specific implementation, and how it fits into the larger architecture of the code base or project before pushing or merging.

---

## 3. Productivity Benefits of AI Coding Tools

**Source:** Peng, S., Kalliamvakou, E., Cihon, P., & Demirer, M. (2023). *The Impact of AI on Developer Productivity: Evidence from GitHub Copilot.*

[Read the research paper](https://arxiv.org/abs/2302.06590)

### Key Findings

Researchers conducted a controlled experiment trying to see exactly how GitHub Copilot affected developer productivity.Participants were asked to implement an HTTP server using JavaScript. The group using GitHub Copilot completed the task approximately **55.8% faster** than the group without AI assistance. This is a good example of a measurable statistic that shows how AI tools can improve the efficiency in the software development process. 

### Limitations

The experiment focused on a specific programming task rather than long-term development in a large existing codebase. The results should not be interpreted as evidence that AI improves productivity by the same amount for every developer or software project.

### Application to This Project

This article is another example that shows how AI coding tools can be valuable resources for software developers.My overall goal for this repository is not to discourage AI usage, but to promote responsible practices that allow developers to take advantage of productivity improvements without sacrificing code quality or understanding. 

---

## 4. Limitations of AI-Assisted Developer Productivity

**Source:** Becker et al. (2025). *Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity.* METR.

[Read the original study](https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/)

[Read the February 2026 update](https://metr.org/blog/2026-02-24-uplift-update/)

### Key Findings

In a 2025 randomized study, METR followed 16 experienced open source developers completing 246 programming tasks. The researchers found that developers who were allowed to use AI tools took approximately **19% longer** to complete their tasks. These developers primarily used Cursor with Claude models rather than the current version of Codex.I thought that this was an interesting finding since AI coding tools are constantly being advertised as ways to improve developer productivity. Even though these developers had access to AI assistance they actually ended up taking more time to finish their work.

Note: METR also published an update in February 2026 that suggested newer AI tools were likely helping developers complete tasks faster. However, the researchers had problems with participant and task selection that made it difficult to accurately measure these improvements.

### Limitations

One important limitation of the original study is that the developers chosed for the expiriment were working on code bases that they already had expirience with and understanded. The February 2026 update also had limitations since developers who preferred using AI were less willing to participate in an experiment where they might have to work without it. This made it difficult for the researchers to accurately measure the productivity benefits of newer AI tools.

### Application to This Project

I thought that this research was useful since it challenged the assumption that using AI will automatically make developers more productive.From my own experience using Codex for programming assignments I have found it to be a useful tool for debugging, writing code, and understanding any code that is unfamiliar to me. However I have also found that verifying code and assertions from AI tools also takes time.I want to encourage developers to evaluate whether using AI is actually beneficial for the task they are completing. I believe that in order to truly utalize the productivity benefits that these tools can offer, developers need to take the time before starting a project to detirmin which parts should include AI assistance. 


## 5. Secure Software Development Standards

**Source:** Souppaya, M., Scarfone, K., & Dodson, D. (2022). *Secure Software Development Framework (SSDF) Version 1.1: Recommendations for Mitigating the Risk of Software Vulnerabilities.* National Institute of Standards and Technology.

[Read the NIST framework](https://csrc.nist.gov/pubs/sp/800/218/final)

### Key Findings

The National Institute of Standards and Technology developed a specfic framework for secure software development. The framework emphasizes secure development practices, identifying vulnerabilities, and verifying software before release. This framework was not  designed for AI-assisted software development, however I believe that many of the recommendations included in it are extremely relevant when AI tools are used to generate or modify code.

### Limitations

The framework is designed for a general software development instead of smaller student development teams. Some practices may require additional resources or formal processes that are not really practical for small educational projects.

### Application to This Project

I plan to use this framework as a foundation for the security and verification portions of my guidelines. However, I want to adapt these practices to my actual audience of UCSB Computer Science students. Rather than requiring complicated professional security procedures, my guidelines will focus on realistic practices such as checking user input, protecting sensitive information, reviewing changes, and testing important functionality before merging code.

---

## How This Research Influences the Guidelines

| Research Finding | Guideline or Workflow Recommendation |
|---|---|
| AI assistance can introduce security vulnerabilities. | Independently review AI-generated code for security concerns. |
| Developers may struggle to understand generated solutions. | Require developers to explain their implementations before merging. |
| AI can improve productivity on certain tasks. | Encourage AI assistance when it provides a practical benefit. |
| AI does not consistently improve productivity in every environment. | Evaluate when using AI is actually appropriate. |
| Secure development requires verification throughout the process. | Include human review, testing, and security checks in the development workflow. |

## Conclusion
Throughout all of the research I review, the sources that I have included help provide examples and practices that pertain to responsible AI-assisted software development. As always AI tools should act as a support mechanism instead of a crutch when developing software. AI should never replace a developers judgement or understanding of what they are developing. The guidelines and workflow inside of this repository are designed to aid developers in taking advantage of the benefits AI tools can bring while minimizing the downsides. 

