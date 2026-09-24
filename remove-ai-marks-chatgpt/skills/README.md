# Remove AI Marks - ChatGPT Skill

A custom ChatGPT Skill experiment designed to reduce common AI-writing
patterns and produce clearer, more natural-sounding language while
preserving the original meaning and intent.

## Overview

`remove-ai-marks-chatgpt-v2` explores how reusable ChatGPT Skills can be
used to apply a consistent writing-refinement workflow.

The goal is not simply to make text "sound human." Instead, the Skill is
designed to identify and reduce writing patterns commonly associated
with generic AI-generated copy, including:

-   Overly polished or formulaic phrasing
-   Unnecessary buzzwords
-   Generic introductory language
-   Repetitive sentence structures
-   Excessive abstraction
-   Inflated or vague claims
-   Unnatural transitions
-   Unnecessary verbosity

The intended result is writing that feels clearer, more direct,
conversational, and specific without changing the author's underlying
meaning.

## Example

**Original**

> In today's rapidly evolving digital landscape, organizations must
> leverage innovative solutions to unlock their full potential.

**Intended refinement**

> As technology changes, organizations need practical ways to adapt and
> make better use of the tools available to them.

The refinement removes phrases such as "rapidly evolving digital
landscape," "leverage innovative solutions," and "unlock their full
potential" in favor of more direct language.

## Why I Built This

AI is increasingly useful as a writing and creative partner, but
generated copy can develop recognizable patterns when the language
becomes too polished, generic, abstract, or predictable.

Rather than manually correcting those patterns every time, I wanted to
explore whether the process could become a reusable workflow.

This project is an experiment in:

-   Prompt and instruction design
-   Reusable AI workflows
-   ChatGPT Skills
-   AI-assisted writing refinement
-   Workflow packaging
-   Human + AI collaboration
-   Testing emerging AI platform capabilities

It also reflects a broader principle behind my AI workflow work:

> **Build once. Improve forever.**

When a useful process emerges repeatedly, the goal is to turn it into
something reusable rather than recreate it from scratch each time.

## Project Structure

``` text
remove-ai-marks-chatgpt-v2/
├── SKILL.md
├── README.md
└── supporting skill files
```

`SKILL.md` contains the primary instructions that define how the Skill
should perform the writing-refinement workflow.

Supporting files may contain additional guidance, examples, or resources
used by the Skill.

## Current Status

**Experimental / Platform Testing**

The Skill package was successfully accepted and displayed as installed
by ChatGPT.

However, during testing on **September 24, 2026**, a newly created
ChatGPT conversation was unable to discover or invoke the installed
custom Skill through the model's available Skills runtime.

### Observed behavior

1.  The custom Skill package was created and packaged for ChatGPT.
2.  ChatGPT accepted the package.
3.  The Skill appeared as installed in the ChatGPT interface.
4.  A new conversation was created after installation.
5.  The model's available Skills were queried.
6.  `Remove AI Marks` was not exposed as an available Skill and
    therefore could not be invoked.

This suggests that successful installation in the interface does not
necessarily mean a user-installed custom Skill is currently available to
the active model/runtime.

Because ChatGPT Skills and related capabilities are evolving, this
behavior may change.

## Why Keep an Experiment That Doesn't Fully Work Yet?

The experiment itself is useful.

This repository preserves:

-   The Skill architecture
-   The writing-refinement methodology
-   The packaged implementation
-   The testing process
-   The observed platform limitation
-   A baseline that can be retested as ChatGPT's Skills capabilities
    evolve

Documenting unsuccessful or partially supported experiments is part of
understanding emerging AI tools.

The result isn't just the artifact---it's what the experiment teaches
about how the platform actually behaves.

## Future Exploration

Potential next steps include:

-   Retesting the Skill as ChatGPT's custom Skills support evolves
-   Refining the instruction architecture
-   Expanding before/after examples
-   Testing the workflow across different writing styles
-   Comparing Skill-based execution with standard prompting
-   Exploring similar reusable workflows for design and creative
    production

## Related Project

This experiment is part of my broader **AI Design Workflows**
repository, where I explore practical ways to integrate AI into design,
writing, creative production, and repeatable workflows.

The focus is not AI for its own sake, but finding places where AI can
make creative work clearer, faster, more consistent, or easier to
maintain.

------------------------------------------------------------------------

**Status:** Experimental\
**Version:** v2\
**Last tested:** September 24, 2026
