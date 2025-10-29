---
layout: page
permalink: /keynote/
title: Keynote speech
nav: true
nav_order: 2
---

## Keynote

### "How to Write Secure Programs with LLMs"
<br>
{% include people_horizontal.html name="Prof. Hyoungshick Kim" affiliation="Sungkyunkwan University, Republic of Korea" img="/assets/img/hyoung_hp1.jpg" %} 

**Bio.** Hyoungshick Kim is a professor in the Department of Computer Science
and Engineering at Sungkyunkwan University. He received a BS degree
from the Department of Information Engineering at Sungkyunkwan
University, an MS from the Department of Computer Science at KAIST,
and a Ph.D. from the Computer Laboratory at the University of
Cambridge in 1999, 2001, and 2011, respectively. After completing his
Ph.D., he worked as a post-doctoral fellow in the Department of
Electrical and Computer Engineering at the University of British
Columbia. He previously worked as a senior engineer at Samsung
Electronics from 2004 to 2008. He also worked as a distinguished
visiting researcher at CSIRO Data61 from 2019 to 2020.

His current research interests include usable security, software
security, and data-driven security. He enjoys finding security issues
in new systems, particularly recent AI systems and applications, and
has been deeply engaged in identifying real security problems in these
areas. His work aims to uncover and address the practical security
challenges posed by emerging technologies.


**Keynote Abstract.** AI coding assistants, such as GitHub Copilot and Cursor, have quickly
become an integral part of developers' everyday workflows, but how
safe is the code they generate? In this talk, I'll dive into what
makes AI-generated code insecure, drawing on recent case studies and
experiments that show about 40% of LLM-generated code contains
vulnerabilities.

I'll examine four root causes of insecure code generation:
contaminated training data, security-blind prompts, lack of
vulnerability detection, and limited understanding of security
semantics. Then I'll walk through current efforts to address these
issues using fine-tuning (achieving up to 56% reduction in
vulnerabilities), prompt engineering (up to 69% fixes through
iterative prompting), and retrieval-augmented techniques with
community knowledge bases like Stack Overflow.

I'll also present our own approach to automated vulnerability repair:
San2Patch, which leverages vulnerability logs and tree-of-thought
reasoning to achieve 79.5% patch success on known CVEs and
successfully repairs real-world vulnerabilities in under 9 minutes.
However, I'll also discuss the fundamental limitations we've
encountered—repository-level program repair remains challenging for
current LLMs, with only 54% success even with direct zero-shot
prompting.

This talk highlights both the potential and the current gaps in making
large language models truly helpful for secure programming. The
ultimate goal is to move beyond fixing bugs to actually teaching
models why code is secure—not just what secure code looks like.

