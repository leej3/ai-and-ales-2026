# My agent workbench

Five-minute speaking script for John Lee.
AI & Ales, Jamestown Frontier Society, October 15, 2026.

## 1. My agent workbench (0:00–0:25)

I'm John.
I work on research software at Dartmouth's Center for Open Neuroscience.
I use coding agents to build software, explore ideas, and prepare talks like this one.
Tonight I want to show a few things I've made and the question connecting them: when an agent produces something, what would let another person understand it and trust it?

Sources:

- https://leej3.github.io/software-engineer-reborn/

## 2. The tools around my agent (0:25–1:10)

The agent is only part of my setup.
Codex works with the actual project files and terminal.
Skills are reusable instructions for a particular kind of work, while Markdown keeps the goal and important decisions visible.
Git records changes.
Worktrees let me try things separately without mixing unfinished changes together.
Pixi describes the software environment, and DataLad connects data and code with their history.
When I need execution records, duct captures what a command did.
These tools give the agent something concrete to act on, and give me something concrete to check.
The skill workshop and worktree utilities are linked here if you want to explore them.

Sources:

- https://github.com/leej3/software-engineer-reborn/tree/main/talk-concepts/06-the-ai-era-development-environment.md
- https://github.com/leej3/skills-workshop
- https://github.com/leej3/stamped-ai-research/tree/codex/stamped-poster-study

## 3. The Software Engineer Reborn (1:10–1:55)

This is The Software Engineer Reborn, a talk I prepared for the Williamsburg software community.
On the left is the preparation: a Talk Atlas where I can compare possible narratives and follow source notes.
On the right is the presentation that came out of that process.
Making a tool to think with became part of making the talk.
The question I kept coming back to was about my own role.
As the machine produces more implementation, I spend more attention on defining the problem, selecting evidence, and deciding which work I can actually stand behind.
Both the preparation and the finished slides are public.

Sources:

- https://software-engineer-reborn-atlas.johnlee3728739.chatgpt.site/
- https://leej3.github.io/software-engineer-reborn/
- https://github.com/leej3/software-engineer-reborn/tree/main/talk-concepts

## 4. What did we just make? (1:55–2:40)

The next talk asks, 'What did we just make?'
A figure or a report is only the visible result.
The useful object also includes the inputs, code, decisions, and environment needed to inspect it or run it again.
Our team's STAMPED principles give us a vocabulary for that package: self-contained, tracked, actionable, modular, portable, ephemeral, and distributable.
In plain terms: can I get the pieces, see their history, run the procedure, and recover a useful state somewhere else?
This matters beyond science.
An AI-generated website, spreadsheet, or presentation also needs enough context for the next person to understand what they have.

Sources:

- https://research-object-with-ai.pages.dev/
- https://github.com/leej3/research-object-with-ai
- https://stamped-principles.org/

## 5. Orinoco Lite: connected research information (2:40–3:35)

Orinoco Lite is one example of software I've been working on with agents.
Research groups have information about people, projects, publications, and software scattered across many places.
Here those things become structured records with explicit relationships.
The website and this graph are different views of those records.
An editor can propose a change through GitHub so the proposal and its review have a visible history.
It builds on the upstream ORINOCO work, with a lighter Git-backed deployment.
What interests me is the shared context: people can browse it, software can validate it, and agents can work with a clearer description of what the group knows.
The screenshot is saved here, so this example doesn't depend on tonight's Wi-Fi.

Sources:

- https://github.com/ORINOCO-Lite/orinoco-lite-dev
- https://dev.centerforopenneuroscience.org/explore/
- https://doi.org/10.5281/zenodo.22834595

## 6. STAMPED in Practice (3:35–4:35)

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

## 7. What would convince you? (4:35–5:00)

That's the thread through my work: agents let me make more things, and I want the result to carry enough evidence for someone else to inspect it.
I'm still figuring out how much context is useful and when keeping it becomes more work than it saves.
I'd love to hear what evidence you look for before trusting something an agent made.
All the projects and this deck's editable source are linked here.

Sources:

- https://github.com/leej3/ai-and-ales-2026
