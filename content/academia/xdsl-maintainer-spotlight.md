---
name: Sasha Lopoukhine, Mathieu Fehr, Tobias Grosser
institution: University of Cambridge
department: Department of Computer Science and Technology
projectName: xDSL
projectRepo: https://github.com/xdslproject/xdsl/
projectWebsite: https://xdsl.dev/
maintainerProfiles:
  - github: http://github.com/tobiasgrosser
  - orcid: https://orcid.org/0000-0003-3874-6003
badges: ["Academic Maintainer"]
description: "An accessible, high-productivity compiler framework for experienced and new compiler developers, compatible with MLIR and used in academia and industry for teaching, research, and production compiler development."
---

## What is xDSL, and what does it help people do?

xDSL is an accessible, high-productivity compiler framework for experienced and new compiler developers. Thanks to its compatibility with [MLIR](https://mlir.llvm.org/) (Multi-Level Intermediate Representation), its users can tap into LLVM's rich ecosystem of production compilers and backends. xDSL is used in both academia and industry for teaching, research and production compiler development. Industry partners who value developer productivity and Python ecosystem integration have repeatedly chosen xDSL as the foundation of their industry-grade software products.

xDSL leverages Python's portability and ease of installation to minimize setup overhead and enable rapid iteration to both students and domain experts. Type hints and extensive testing ensure efficient editing and high code quality. xDSL's interactive compilation environments (e.g., xdsl-gui and Python notebooks) enable developers to explore transformations in a responsive and visual setting.

xDSL uses the same textual representation of programs as MLIR, making it easy to combine both frameworks while maintaining compatibility through continuous integration. This enables research and development across the entire compilation stack, from domain-specific optimisations for large-scale computing to low-level assembly representations for specialised hardware.

## What inspired you to start this project?

Development speed in compiler design had become an innovation bottleneck in academia and central for the success of innovative hardware companies. Existing C++-based compiler frameworks optimized heavily for minimal compile-time performance, but often at the expense of developer productivity and accessibility.

While MLIR's novel multi-level approach revolutionized the design of neural network compilers in industry, MLIR's innovations remained less accessible for academic users and industrial stakeholders targeting Python-based developer communities. The complexity of C++ projects and the overheads they introduce for prototyping prevented the wider use of a state-of-the-art MLIR-style compiler design.

We designed xDSL to answer the question: can we build production-style compilers that make developer productivity a first-class objective?

## How does this project connect to your academic work?

xDSL was born as a collaborative research project between the University of Edinburgh (then Cambridge), EPCC, and Imperial College London. Principal investigators [Tobias Grosser](https://grosser.science/), [Michel Steuwer](https://steuwer.info/), [Nick Brown](https://www.epcc.ed.ac.uk/about-us/our-team/dr-nick-brown), [Amrey Krause](https://www.epcc.ed.ac.uk/about-us/our-team/dr-amy-krause), [Gerard Gorman](https://profiles.imperial.ac.uk/g.gorman), and [Paul Kelly](https://profiles.imperial.ac.uk/p.kelly) kicked off a project that aimed to improve the architecture of the [Devito](https://github.com/devitocodes/devito) and [PSyclone](https://www.esiwace.eu/p-syclone/) HPC compilers, which led to work on accelerated stencil computations on [GPUs](https://dl.acm.org/doi/10.1145/3620666.3651344) and the [Cerebras Wafer-Scale Engine](https://dl.acm.org/doi/10.1145/3779212.3790124) as well as our key idea of [federated compilation with xDSL](https://dl.acm.org/doi/10.1145/3696443.3708945) (published at ASPLOS and CGO). In addition, an active research collaboration was formed and numerous follow-up projects were seeded.

As a cornerstone of the Horizon Europe [CONVOLVE](https://convolve.eu/) compiler workpackage, xDSL developed into a sizable open-source project. At conferences such as CGO, PLDI, and ASPLOS, we published papers on [new ISA-level backend abstractions](https://dl.acm.org/doi/10.1145/3696443.3708952), [first-class verification dialects for MLIR](https://dl.acm.org/doi/10.1145/3729309), and [accelerator configuration overhead modeling](https://dl.acm.org/doi/10.1145/3760250.3762225). Several of our ideas were first prototyped in xDSL and subsequently upstreamed to LLVM, for example the MPI, SMT and (soon) ISA dialects in MLIR. Our CONVOLVE partners (e.g., [KU Leuven](https://micas.esat.kuleuven.be/team/marian-verhelst), [Universidad de Murcia](https://webs.um.es/alexandra.jimborean/miwiki/doku.php), …) as well as other EU projects provided valuable input through their research use of xDSL. This collaboration was reinforced through dedicated xDSL workshops (e.g. ASPLOS and HiPEAC) and hands-on development activities such as the CONVOLVE compiler hackathon, where xDSL was used to support joint experimentation, integration, and co-design across partners.

Overall, xDSL streamlined our own research, led to significant research collaborations, and enabled many external researchers to collaborate with us.

## Who contributes to the project?

xDSL is maintained by a team of students, academics, and industry experts. Increased adoption in production compilers attracts additional open-source contributions. With over 5,000 commits from 125 contributors in total and 34 active contributors in the last 6 months (half of whom had not made prior contributions) the xDSL community grows steadily. Students who leverage xDSL for their dissertation projects frequently upstream changes that would be useful to the broader xDSL community, which leads to a continued inflow of academic contributors.

## How are students involved in the project?

PhD students and postdocs are instrumental to the development of xDSL and take on central leadership roles. Their responsibilities include development, code reviews, communication, and even logo and website design. We are frequently approached by students entering compiler development, who often become active members of the project. xDSL serves students as an entry point into both compilers and collaborative open-source software engineering.

## How is the project used in teaching or coursework?

xDSL is used in teaching compilers in universities and industry. It is used in introductory compiler courses at University of Edinburgh and TU Berlin. We co-organised two MLIR schools in [winter](https://mlir-school.github.io/summer-2025/past_editions/) and [summer 2025](https://mlir-school.github.io/summer-2025/), which leveraged our interactive xDSL-based tutorial notebooks as an introduction to MLIR-style compiler development. The upcoming [2026 MLIR School](https://mlir-school.github.io/summer-2026/) (Aug 2026 - during the solar eclipse in Spain) will also feature an introduction to MLIR using xDSL.

## What impact has this project had on your students?

xDSL has served as a foundation for a number of research papers and dissertations. Doing research in an open-source project improves collaboration opportunities, and increases visibility in industry.

We collected some quotes:

> "xDSL provided the infrastructure that made my doctoral research into tensor data-layout optimization tractable. It enabled highly productive development of experimental intermediate representation design to be paired with existing backend compiler support built into LLVM. I have continued to work with xDSL at Riverlane where we are building compilation tools for quantum error correction that are developed by quantum researchers and FPGA specialists alike. xDSL has provided a toolset that helps to bring these disciplines together, taking advantage of Python's large ecosystem and MLIR's rigorous compiler model."
>
> — Edward Stow, Former PhD student at Imperial College London, Today at Riverlane

> "In our research, we are using xDSL to quickly iterate on the design of [Tamagoyaki](https://github.com/jumerckx/Tamagoyaki), an equality saturation framework that tightly integrates with existing compiler infrastructure. In contrast to MLIR, which is a vast and complex C++ codebase, xDSL is more approachable, and allows us to focus on our research contributions more directly."
>
> — Jules Merckx, PhD student at Ghent University

> "xDSL was my introduction to compilers. It was incredibly approachable and gave me the confidence to dive deeper into the field. Through it, I created "xdsl-gui," now part of the xDSL ecosystem, as my first attempt at interactive compilation tooling. It visualizes pass application, streamlines pass selection by filtering irrelevant options, and provides real-time IR and performance feedback to help measure optimization impact. xDSL genuinely empowered me and kickstarted my compiler journey. I probably would have had a very different experience if my first exposure had been a more heavyweight system. Later, transitioning to MLIR and related tooling felt smooth thanks to the foundation I built with xDSL."
>
> — Dalia Shaaban, Master Student at ETH Zurich

## What impact has the project had beyond the classroom or research?

xDSL is seeing growing adoption in industry. It is used for neural network compilation by AI accelerator startups (engineers from [Synthara](https://synthara.ai/) have recently been making contributions to xDSL), and is used in Google's [LiteRT](http://github.com/google-ai-edge/LiteRT) framework. It is also gaining traction in the quantum compilation space, and is used by [Riverlane](https://www.riverlane.com/), [Xanadu's PennyLane](https://github.com/PennyLaneAI/pennylane) compiler, and [Eclipse's Qrisp](https://github.com/eclipse-qrisp/Qrisp). xDSL's use of Python's type system for compile-time type checking was cited as a motivating example in [PEP 747](https://peps.python.org/pep-0747/). Last year, xDSL was added to the [CPython performance suite](https://github.com/python/pyperformance/tree/b5dfaee6d4da542dc58b2070e018d8449d60d7d9/pyperformance/data-files/benchmarks/bm_xdsl), helping Python core developers optimise typical compiler workloads.

## What does it take to maintain the project?

The project is primarily maintained by two PhD students and two researchers in my group, with additional contributions from other students, researchers, and engineers both inside and outside the group. Over the last year, we've had approximately four commits a day, with a median PR review time of around 10.5 hours.

Contributor onboarding is supported by a detailed "getting started guide", "good first issues" labels, and a robust CI infrastructure. The framework has published 95 releases, and follows a weekly release cycle on PyPI.

## What have been the biggest challenges in maintaining the project, especially in an academic setting?

The most significant challenges occurred in the early stages of the project, when a large amount of functionality was required to reach compatibility with MLIR.

Now that this foundation is more stable, contributions can happen in the background and require less time relative to research work. Changes are made and reviewed by students and researchers in the team, allowing them to integrate smoothly alongside other responsibilities.

## How do you ensure the project remains sustainable over time?

Sustainability largely comes from shared ownership. As more research groups and industry adopt xDSL, they contribute improvements and maintenance back to the project. This collaborative open-source model helps distribute the long-term maintenance effort across the community.

## How do you engage with your community?

We maintain a website and documentation, alongside GitHub Discussions and an open Zulip chat, with 159k total messages and an average of 30 daily active users. We run weekly meetings that are open to the xDSL community, where we discuss ongoing topics in the development and maintenance of xDSL.

We also provide guidance on pull request formatting and onboarding. On a new member's first day, an existing team member helps them open their first pull request, ensuring early engagement.

## Have you taken part in any open source programs or events?

Not yet, but we would be interested in participating in the future.

## What would you love to achieve by showcasing your project?

The project is inherently social and becomes more useful as its user base grows. We hope that showcasing it will encourage more people to try it and contribute. In fact, we want to encourage design choices that challenge conventional wisdom, like the idea of writing a compiler in Python. While not the obvious choice for a traditional compiler engineer, the new design point xDSL chose has led to significant innovation which also regularly feeds back to the LLVM community.

## Is there anything else you'd like to share about your project or open source journey?

My (Tobias') personal academic career started with open-source development and led to a strong desire to perform open-source-first research. I began contributing to open source over 15 years ago as a GCC developer, when I joined the Graphite research project led by Sebastain Pop and Albert Cohen. Since my first day as a student, open source has played a major role in shaping my career. In fact, I wrote almost exclusively open-source code, most of which either became part of or initiated an open-source project. Mathieu and Sasha both develop large-scale open-source projects as core part of their PhD, and give students with xDSL every day the opportunity to engage in open-source-focused research. For us, open-source research is engaging, productive, and incredibly social. We thank the xDSL and wider open-source community for the welcoming and engaging atmosphere they offer!
