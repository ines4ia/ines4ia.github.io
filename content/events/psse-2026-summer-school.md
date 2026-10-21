---
title: "Third Pernambuco Summer School on Software Engineering (AI×SE 2026)"
date: 2026-10-09
dateLabel: "December 7–11, 2026"
pinned: true
pinnedUntil: 2026-12-11T23:59:59-03:00
tag: "Summer School"
image: "/img/events/summer-school-2026.svg"
summary: "AI-Driven Software Engineering: Challenges and Opportunities — December 7–11, 2026, Japaratinga, Alagoas, Brazil."
---

## Overview

The **Third Pernambuco Summer School on Software Engineering (AI×SE 2026)** is a five-day intensive school bringing together leading researchers and practitioners to explore the rapidly evolving intersection between Artificial Intelligence and Software Engineering. The school welcomes **academic researchers, PhD and MSc students, and industry practitioners** who are interested in understanding and shaping how AI is transforming software engineering practice and research.

The school is organized by the **Informatics Center (CIn)** of the **Federal University of Pernambuco (UFPE)**.

AI is fundamentally reshaping how software is conceived, built, tested, and maintained. Large language models now generate, explain, and refactor code; autonomous agents navigate complex engineering workflows with minimal human supervision; and empirical studies are increasingly powered by AI-based analysis pipelines. At the same time, Software Engineering methods (formal specification, testing theory, program analysis, and human factors) provide the rigorous foundations that AI-based systems urgently need. This school addresses *both* directions: AI as a tool for engineering software, and Software Engineering as a discipline for building trustworthy AI.

## Goals

- Expose researchers and practitioners to cutting-edge topics at the AI×SE intersection.
- Foster interactions between participants and invited lecturers from academia and industry.
- Provide a forum for participants to present and receive feedback on their research and practical experiences.
- Stimulate new research collaborations and industry–academia partnerships within the Brazilian and international communities.

## Invited Lecturers

<div class="lecturers">
<div class="lecturer">
  <h3 class="lecturer-name"><a href="https://ruimaranhao.com/">Rui Abreu</a></h3>
  <p class="lecturer-affil">Meta &amp; University of Porto, Portugal</p>
  <p class="lecturer-talk">Risk-Aware Software Engineering: Predicting Failure Before Code Lands</p>
  <details class="lecturer-abstract">
    <summary>Abstract</summary>
    <p>Every code change is a bet on production. Most land safely; a few cause severe incidents (SEVs) that are expensive, disruptive, and hard to anticipate from the pull request (diff) alone. This course presents the Diff Risk Score (DRS), an AI-powered system developed at Meta that predicts, before a change lands, how likely it is to cause a production incident. Built on fine-tuned Llama models, DRS reads the diff and its metadata and assigns a continuous risk score, highlighting the lines and hunks that drive it. We cover the full pipeline: formulating SEV prediction as a learning problem, calibration and percentile-based gating, and deployment at scale. Low-risk diffs bypass traditional bottlenecks such as code freezes, while the riskiest changes are routed to deeper review and specialised workflows such as the Risky Diff Reviewer. We then turn to explainability, using attention to show why a change is flagged, and close with open problems: configuration risk, agentic mitigation, and the fundamental trade-off between shipping fast and staying reliable.</p>
  </details>
  <details class="lecturer-abstract">
    <summary>Bio</summary>
    <p>Rui Abreu is with Meta and the University of Porto (FEUP), Portugal, where he is a Full Professor of Software Engineering. His research focuses on software testing and fault diagnosis, software security and vulnerability detection, AI-assisted software engineering — including risk prediction for code changes at scale — and quantum software engineering. He was previously an Associate Professor at Instituto Superior Técnico (University of Lisbon), a Visiting Researcher at Google NYC, a Member of Research Staff at Xerox PARC, a Visiting Faculty Member at Carnegie Mellon University, and the founding Head of Engineering at DashDash/Rows. He holds a Ph.D. in Computer Science from Delft University of Technology (2009). His work has received several best paper awards, including an ACM SIGSOFT Distinguished Paper Award at ESEC/FSE 2019, and he is an IEEE Senior Member.</p>
  </details>
</div>
<div class="lecturer">
  <h3 class="lecturer-name"><a href="http://monperrus.net">Martin Monperrus</a></h3>
  <p class="lecturer-affil">KTH Royal Institute of Technology, Sweden</p>
  <p class="lecturer-talk">Software Engineering in the Latent Space</p>
  <details class="lecturer-abstract">
    <summary>Abstract</summary>
    <p>Programs are symbolic objects, discrete, structured and executable. Yet inside large language models, programs, bugs, patches, tests and specifications exist implicitly as vectors. This course introduces software engineering in the latent space, which revisits core software engineering problems by working directly on these internal representations. The guiding hypothesis is a duality between symbolic programs and their continuous counterparts, in which latent geometry faithfully captures program semantics. If the duality holds, a gradient step could move toward a bug fix before a single token is written. We cover representation: the residual stream, the linear representation hypothesis, and rigorous probing. We then ask what code models encode about types, data flow, execution state and bugs, and whether those encodings stay stable across models, languages and semantics-preserving rewrites.</p>
  </details>
  <details class="lecturer-abstract">
    <summary>Bio</summary>
    <p>Martin Monperrus is Professor of Software Technology at KTH Royal Institute of Technology, Sweden, where he holds a Chair from the Wallenberg Autonomous Systems and Software Program (WASP). His research focuses on AI-assisted coding, automated program repair, and software engineering. He was previously an associate professor at the University of Lille and affiliated researcher at Inria (France), and a research associate at Darmstadt University of Technology (Germany). He holds a Ph.D. from the University of Rennes (2008). His 2009 paper on learning-based code completion, co-authored with Marcel Bruch and Mira Mezini, laid the foundations for tools such as GitHub Copilot and received the ACM SIGSOFT Impact Paper Award (2024); he was elevated to IEEE Fellow (Class of 2026).</p>
  </details>
</div>
<div class="lecturer">
  <h3 class="lecturer-name"><a href="https://www.softlang.org/rlaemmel:home">Ralf Lämmel</a></h3>
  <p class="lecturer-affil">University of Koblenz, Germany</p>
  <p class="lecturer-talk">AI-Based Software Vulnerability Detection</p>
  <details class="lecturer-abstract">
    <summary>Abstract</summary>
    <p>The increasing adoption of Artificial Intelligence (AI) in software engineering is reshaping how software vulnerabilities are identified and assessed. Learning-based approaches, ranging from pretrained code representations to Large Language Models (LLMs), promise to complement traditional static analysis by capturing complex patterns in source code. Yet, despite impressive benchmark results, fundamental questions remain about what these models actually learn, how reliably they distinguish vulnerable from secure code, and whether their capabilities generalize beyond the data on which they were trained.</p>
    <p>This lecture series provides a structured exploration of AI-based software vulnerability detection, progressing from foundational concepts and practical methods to advanced research on model representations and generalization. We begin by comparing learning-based vulnerability detection with conventional static analysis, examining their respective strengths, limitations, and underlying assumptions. We then discuss the construction and characteristics of vulnerability datasets, common evaluation pitfalls, and baseline detection approaches using CodeBERT and LLMs.</p>
    <p>Interactive hands-on lab sessions accompany the lectures, allowing participants to directly inspect models, datasets, and representation metrics in code.</p>
    <p>Building on these foundations, the lectures introduce deeper concepts in representation learning, including embedding geometry, contrastive learning, and out-of-distribution (OOD) detection. Particular attention is given to how the structure of learned representations can reveal model behaviour that, for example, internal LLM confidence metrics fail to capture.</p>
    <p>The series culminates in a detailed case study investigating the <strong>generalization boundaries of AI-based vulnerability detection</strong>. Through carefully controlled experiments involving vulnerable and patched code pairs, we examine how CodeBERT and Qwen2.5-Coder behave under shifts in vulnerability patterns, software projects, and time. We explore how calibrated embedding geometry can expose unfamiliar inputs, characterize degradation in detection reliability, and explain characteristics of false positives.</p>
    <p>Ultimately, the lecture series aims to bridge practical AI-based vulnerability detection with a deeper understanding of <strong>when, why, and how learned models fail to generalize</strong>.</p>
    <p><em>Acknowledgement:</em> The material for the lecture series was prepared jointly with Konstantin Ievtushenko (SoftLang Team), also drawing from his recently completed MSc thesis. The final study on the generalization boundaries in AI-based vulnerability detection is available as a preprint: <a href="https://arxiv.org/abs/2610.14296">arXiv:2610.14296</a> (Konstantin Ievtushenko, Ralf Lämmel, and Jan Jürjens; under review).</p>
  </details>
  <details class="lecturer-abstract">
    <summary>Bio</summary>
    <p>Ralf Lämmel is Professor of Computer Science at the University of Koblenz, Germany, where he leads the Software Languages research group. His research focuses on software language engineering, program transformation, reverse and re-engineering, program comprehension, and model-driven engineering, and more recently on knowledge graphs, ontologies, and the use of AI in software engineering. He has held research and engineering positions at Facebook (Meta), Microsoft, Vrije Universiteit Amsterdam, CWI (the Netherlands), the University of L'Aquila, and the University of Rostock. He is a co-founder of the Software Language Engineering (SLE) conference and the GTTSE summer school series, and the author of <em>Software Languages: Syntax, Semantics, and Metaprogramming</em> (Springer, 2018), a Choice Outstanding Academic Title in 2019.</p>
  </details>
</div>
<div class="lecturer">
  <h3 class="lecturer-name"><a href="https://gustavoasoares.github.io/">Gustavo Soares</a></h3>
  <p class="lecturer-affil">Google</p>
  <p class="lecturer-talk">Agentic Engineering in Practice: Lessons from Building AI Developer Tools</p>
  <p class="lecturer-pending">Abstract coming soon.</p>
  <details class="lecturer-abstract">
    <summary>Bio</summary>
    <p>Gustavo Soares is with Google. His research focuses on program synthesis techniques and tools to help developers, students, and end users, including learning program transformations from examples. He was previously a Researcher at Microsoft, working in the PROSE team, an assistant professor at the Federal University of Campina Grande (UFCG), Brazil, and a postdoctoral visiting researcher at UC Berkeley. He holds a Ph.D. in Computer Science from UFCG (2014), during which he visited North Carolina State University and interned at Microsoft Research. His work on programming-by-example contributed to tools deployed in Windows as PowerShell commands and to the Microsoft PROSE framework.</p>
  </details>
</div>
<div class="lecturer">
  <h3 class="lecturer-name"><a href="https://bvasiles.github.io/">Bogdan Vasilescu</a></h3>
  <p class="lecturer-affil">Carnegie Mellon University, USA</p>
  <p class="lecturer-pending">Title to be announced.</p>
  <details class="lecturer-abstract">
    <summary>Bio</summary>
    <p>Bogdan Vasilescu is an Associate Professor in the School of Computer Science at Carnegie Mellon University, USA, and a member of the Software and Societal Systems Department, where he leads the STRUDEL lab (Socio-Technical Research Using Data Excavation). His research focuses on the socio-technical aspects of software development, including the health and sustainability of open-source ecosystems, diversity and human factors, and the impact of AI on software development practices. He was previously a postdoctoral researcher at UC Davis. He holds a Ph.D. in Computer Science from Eindhoven University of Technology (2014), whose dissertation received the Best Dissertation Award from the Institute for Programming Research and Algorithmics. He co-chaired the MSR 2023 program committee, is an Associate Editor of ACM TOSEM, and received Distinguished Reviewer Awards at ASE 2018 and ESEC/FSE 2021.</p>
  </details>
</div>
</div>

## Venue and Location

The school takes place at the **Bitingui Praia Hotel**, in **Japaratinga**, a small coastal town in the state of Alagoas, Brazil, renowned for its crystal-clear warm waters, coral reefs, and preserved natural beauty.

- **Nearest airports:** Maceió/Zumbi dos Palmares International Airport (MCZ), approximately 90 km from Japaratinga; and Recife/Guararapes–Gilberto Freyre International Airport (REC), approximately 260 km from Japaratinga.
- **Access:** A transfer will be provided only from Recife to Japaratinga. Details will be communicated to registered participants.

Japaratinga is part of the Costa dos Corais (Coral Coast) environmental protection area. The town is known for its tranquil atmosphere, natural pools formed by coral reefs at low tide, and pristine beaches. December brings warm, sunny weather, ideal for an immersive research retreat.

## Organizing Committee

- Augusto Sampaio (CIn / UFPE)
- Paulo Borba (CIn / UFPE)
- Sergio Soares (CIn / UFPE)
- Guilherme Cavalcanti (IFPE)
- Leo Fernandes (IFAL)
- Paola Accioly (CIn / UFPE)
- Rodrigo Bonifácio (CIn / UFPE)
- Thais Burity (UFAPE)

## Contact

For questions regarding the school or registration, please contact the organizing committee at [psse_2026@cin.ufpe.br](mailto:psse_2026@cin.ufpe.br).
