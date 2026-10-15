# My agent workbench

Five-minute speaking script for John Lee.
AI & Ales, Jamestown Frontier Society, October 15, 2026.

## 1. My agent workbench (0:00–0:20)

I'm John.
I work on research software at Dartmouth's Center for Open Neuroscience.
I use coding agents to build software, explore ideas, and prepare talks.
Here are a few things I've made, connected by one question: what would let another person understand an agent's work and trust it?

Sources:

- https://leej3.github.io/software-engineer-reborn/

## 2. The tools around my agent (0:20–0:55)

Codex works with my actual project files and terminal.
Skills are reusable instructions, while Markdown keeps the goal and decisions visible.
Git records changes, and worktrees keep separate experiments from mixing together.
Pixi describes the software environment, and DataLad connects data and code with their history.
When I need execution records, duct captures what a command did.
These tools give the agent something concrete to act on, and give me something concrete to check.
My skill workshop and worktree utilities are linked here.

Sources:

- https://github.com/leej3/software-engineer-reborn/tree/main/talk-concepts/06-the-ai-era-development-environment.md
- https://github.com/leej3/skills-workshop
- https://github.com/leej3/stamped-ai-research/tree/codex/stamped-poster-study

## 3. Keyhatch (0:55–1:30)

Keyhatch tackles a very practical interruption: an agent needs a credential to do useful work.
I'm building a native Mac app where I approve selected credentials once, then allow repeated retrieval during a limited window.
Apple Passwords remains the source of truth, with selective import into Keyhatch.
A local command-line client connects the agent to the broker.
The important tradeoff is that a recipient can keep a disclosed secret.
Expiry stops future retrieval; it cannot take that secret back.
It's an experimental project with public source.
Production signing and release validation remain unfinished.

Sources:

- https://github.com/leej3/keyhatch
- https://github.com/leej3/keyhatch/blob/main/SECURITY.md
- https://github.com/leej3/keyhatch/blob/main/docs/DISTRIBUTION.md

## 4. The Software Engineer Reborn (1:30–2:10)

This is The Software Engineer Reborn, a talk for the Williamsburg software community.
On the left is the preparation: a Talk Atlas for comparing narratives and following source notes.
On the right is the presentation.
Making a tool to think with became part of making the talk.
The question was about my own role.
As the machine produces more implementation, I spend more attention on defining the problem, selecting evidence, and deciding which work I can stand behind.
Both the preparation and the finished slides are public.

Sources:

- https://software-engineer-reborn-atlas.johnlee3728739.chatgpt.site/
- https://leej3.github.io/software-engineer-reborn/
- https://github.com/leej3/software-engineer-reborn/tree/main/talk-concepts

## 5. What did we just make? (2:10–2:50)

The next talk asks, 'What did we just make?'
A figure or report is only the visible result.
The useful object also includes the inputs, code, decisions, and environment needed to inspect or rerun it.
Our team's STAMPED principles give us a vocabulary: self-contained, tracked, actionable, modular, portable, ephemeral, and distributable.
In plain terms: can I get the pieces, see their history, run the procedure, and recover a useful state elsewhere?
This matters beyond science.
An AI-generated website or spreadsheet also needs enough context for the next person.

Sources:

- https://research-object-with-ai.pages.dev/
- https://github.com/leej3/research-object-with-ai
- https://stamped-principles.org/

## 6. Orinoco Lite: connected research information (2:50–3:40)

Orinoco Lite is software I've been working on with agents.
Research groups have information about people, projects, publications, and software scattered across many places.
Here those become structured records with explicit relationships.
The website and this graph are different views of those records.
An editor proposes changes through GitHub, preserving a visible review history.
It builds on upstream ORINOCO with a lighter Git-backed deployment.
What interests me is shared context: people can browse it, software can validate it, and agents can work with a clearer description of what the group knows.
This screenshot is saved, so the example works without Wi-Fi.

Sources:

- https://github.com/ORINOCO-Lite/orinoco-lite-dev
- https://dev.centerforopenneuroscience.org/explore/
- https://doi.org/10.5281/zenodo.22834595

## 7. STAMPED in Practice (3:40–4:35)

The Zenodo record describes the original STAMPED in Practice proposal.
The current poster PR captures the later public-data pilot, with working analyses and concrete failures to learn from.
The next repository develops a repeated improvement process.
Independent agents tackle the same scientific question under four kinds of assistance: baseline, general skill discovery, reproducibility-focused discovery, and explicit STAMPED skills.
Independent judges assess scientific quality separately from how well the research object supports inspection and reuse.
We then improve the skills and try again, keeping assessment fixed within a formal comparison.
NARPS preparation pilots are already exposing useful problems.
The hypothesis is that detailed STAMPED guidance improves performance and reduces inconsistent outcomes.
The goal is transfer: a researcher brings their own data and hypothesis, and an independent agent can use these skills to do rigorous, convenient research.
That improvement remains to be tested.

Sources:

- https://github.com/con/talks/pull/35
- https://zenodo.org/records/22833916
- https://github.com/leej3/stamped-ai-research-next
- https://github.com/leej3/stamped-ai-research-next/pull/3

## 8. What would convince you? (4:35–5:00)

That's the thread through my work: agents let me make more things, and I want the result to carry enough evidence for someone else to inspect it.
I'm still figuring out how much context is useful and when keeping it becomes more work than it saves.
I'd love to hear what evidence you look for before trusting something an agent made.
All the projects and this deck's editable source are linked here.

Sources:

- https://github.com/leej3/ai-and-ales-2026
