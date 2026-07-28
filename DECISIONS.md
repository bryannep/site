# Design Decisions

## Why not a traditional portfolio?

The goal is not to demonstrate experience.

The goal is to demonstrate judgment.

A chronological portfolio centers projects and roles.

This site centers organizational ideas, capabilities, and evidence.

## Why organize around Learn → Align → Decide?

These are the organizational capabilities connecting every stage of the work.

Individual projects are expressions of these capabilities.

## Why projects are supporting evidence

The site leads with a transferable organizational principle.

The project demonstrates that the principle has been implemented in practice.

## Why Field Notes?

Field Notes separate observation from explanation.

They provide judgment and personality without interrupting the main narrative.

## Why Exhibits?

Exhibits allow artifacts to prove capability without becoming the main story.

Supported exhibit types include video, diagram, case study, slide, framework, and document.

Exhibits should be selected based on evidentiary value, not visual availability.

## Why Essays?

Essays extend an idea beyond any single project or organization.

They provide space for deeper thinking while keeping the main site concise.

## Why principle-first writing?

Executives remember ideas.

They use evidence to evaluate those ideas.

The site follows the same pattern.

## Why editorial layouts instead of flat card grids?

Flat grids imply equal importance.

The work does not have equal strategic weight.

Editorial layouts create hierarchy, pacing, and emphasis.

## Why progressive disclosure?

The visible page should remain calm and scannable.

Visitors who want more depth can reveal it through flip cards, expandable Field Notes, embedded exhibits, linked documents, and essays.

## Why every major capability ends with tangible principles

A capability should not end with a generic outcome list.

It should conclude by showing the principles the organization can continue to use.

The pattern is:

**Capability**

↓

**Principles made tangible**

↓

**Exhibits that prove those principles**

This turns the site from a record of completed work into a demonstration of reusable executive judgment.

## Why capability hierarchy matters

Not every contribution should receive equal visual treatment.

The site distinguishes among:

- Anchor capability
- Supporting capabilities
- Supporting ideas or evidence

This directs attention toward the work that best demonstrates executive-level influence and organizational transformation.

## Why five typographic roles?

Earlier iterations accumulated too many component-specific text styles. The resulting hierarchy changed from section to section and forced visitors to repeatedly relearn how to read the page.

The five-role system creates repetition:

- Label
- Display
- Deck
- Body
- Caption

Semantic heading levels remain meaningful, while visual consistency comes from reusable roles and shared spacing.

## Why line-length constraints?

Editorial typography depends on controlled measure.

- Display headlines remain intentionally narrow
- Deck copy stays around 40–52 characters per line
- Body copy stays around 55–68 characters per line

This creates hierarchy without relying on excessive size changes or decorative treatments.


## Why layout controls text width

Earlier versions attempted to control wrapping through nested `max-width` rules on headings and paragraphs. Those rules conflicted with one another and caused text to wrap early despite visible available space.

The revised rule is:

- Layout determines width
- Typography determines appearance
- Content determines natural line breaks

The Philosophy section now uses a two-column grid for narrative and Field Note content, followed by a full-width principle grid.


## Why the Philosophy Field Note is independently positioned

A two-column grid reserved the Field Note width plus gutter across the entire Philosophy introduction. That reduced the narrative measure even where the note did not occupy the same vertical space, producing premature line breaks.

The Field Note is now independently positioned. The narrative uses the full content region, while the artifact remains visually associated with the section.


## Why questions and capability titles share one token

The Philosophy question appeared visually different from the principle titles because it inherited paragraph color even when its size and weight were similar.

Questions, principles, and capability titles now use one shared bold title token. This removes duplicated typography rules and prevents visual drift across sections.


## Why the Systems subsection statements are italic

Learn, Align, and Decide sit beneath the hero-level Systems section.

Their statements are not ordinary headings or project names. They describe the leadership capabilities Bryanne brings to an organization:

- Strengthening organizational learning
- Creating confidence across people, priorities, and products
- Improving decision quality under uncertainty

The italic serif treatment marks each as a subsection thesis while preserving the wording as an expression of leadership identity.

## Why the wording is not forced into grammatical parallelism

The three lines were written to describe what Bryanne does as a leader.

Visual consistency should come from typography and structure, not by rewriting the statements into a more generic pattern.

## Why the hero and Philosophy are protected

Repeated global and section-level CSS changes unintentionally altered the approved hero and Philosophy.

The current rule is that changes below Philosophy must use scoped selectors and must not redefine:

- hero width
- hero headline scale
- hero grid
- Philosophy thesis
- Philosophy narrative width
- Philosophy Field Note placement

## Why current documentation names a single baseline

Multiple experimental HTML versions and accumulated overrides made it difficult to distinguish approved decisions from abandoned experiments.

Version v0.47 is the current source of truth. Future work should branch from this version and record every approved visual or content change in the changelog.
