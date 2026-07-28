# Design Principles

## Emotional Goal

The site should feel:

- Calm
- Rigorous
- Curious
- Human

Visitors should think:

> “I’ve never seen someone explain business problems this way.”

and

> “I want to work with this person.”

## Positioning

This is not a traditional portfolio.

It is an executive field notebook and strategy book.

Projects are evidence.

Ideas are the product.

## Brand Themes

- Executive strategy book
- Field notebook
- Scientific rigor
- Occasional delight

## Visual Language

- Binder clips
- Handwritten Field Notes
- Editorial layouts
- Minimal motion
- System diagrams
- Large typography
- White space
- Tactile paper cues
- Progressive disclosure

## Content Language

### Field Notes

Field Notes are short observations.

They reveal judgment, interpretation, personality, and the thought behind the work.

### Exhibits

Exhibits are supporting evidence.

Exhibits include:

- video
- diagram
- case study
- slide
- framework
- document

### Essays

Essays provide deeper exploration.

They extend ideas beyond any single project, artifact, or organization.

## Content Hierarchy

**Idea**

↓

**Capability**

↓

**Exhibit**

↓

**Field Note**

The site teaches first.

Evidence comes second.

Interpretation adds depth.

## Capability Structure

Every major capability should:

1. Begin with a memorable organizational statement
2. Use a project or program as supporting evidence
3. Show what changed at the organizational level
4. Conclude by making its principles tangible through exhibits

Capabilities should not all receive equal visual weight.

Use hierarchy intentionally:

- Anchor capability
- Supporting capabilities
- Supporting ideas or evidence

## Motion Principles

Animations reveal ideas.

They never decorate.

- Diagrams draw themselves
- Binder clips gently wiggle
- Field Notes slide naturally into view
- Flip cards reveal deeper evidence
- Motion supports sequence, causality, or attention
- Reduced-motion preferences must be respected

## Writing Principles

- Lead with ideas
- Support with evidence
- Never oversell
- Teach
- Reveal judgment
- Favor memorable framing over exhaustive explanation
- Put organizational problems before project descriptions
- Use project names as supporting examples
- Prefer present tense for reusable principles
- Describe organizational capability, not merely activity
- Preserve distinctions among systems, frameworks, methods, visualizations, and artifacts

## Typography

### Editorial

Large serif headlines and strategic framing.

### Interface

Navigation, labels, metrics, and supporting copy.

### Handwriting

Field Note labels, Field Note bodies, and small annotations.

Field Note labels use a firmer handwritten font.

Field Note body copy uses a softer handwritten font.

## Color System

- `#287493` on light backgrounds
- `#7DBCDC` on dark backgrounds
- Black or near-black ink for Field Notes

## Deliberately Avoid

- Generic portfolio templates
- Résumé-style accomplishment lists
- Flat grids that imply equal importance
- Decorative UX language
- Walls of process documentation
- Unexplained artifacts
- Empty metrics
- Excessive animation
- SaaS dashboard aesthetics
- Startup gradients
- Cute elements that reduce credibility
- Treating every contribution as a method

## Five-Role Typography System

The site uses five recurring typographic roles.

### Label

Small uppercase sans-serif text for section labels, content types, dates, and metadata.

Examples:

- PHILOSOPHY
- LEARN
- EXHIBIT 02
- DESIGN WITH US

### Display

Large serif text for the primary thesis of a page, section, or capability.

Examples:

- Organizations don’t struggle because they lack data.
- Better products are a natural outcome of better decisions.
- Strengthening organizational learning.

### Deck

Medium serif text that explains or reframes the display statement.

Deck copy should remain between roughly 40 and 52 characters per line.

### Body

Sans-serif text for narrative explanation, evidence, and supporting detail.

Body copy should remain between roughly 55 and 68 characters per line.

### Caption

Small text for exhibit descriptions, article categories, citations, and secondary context.

## Semantic Heading Rules

- `h1` — the homepage thesis; one per page
- `h2` — major site sections
- `h3` — major questions or pillars within a section
- `h4` — capability statements and principle titles
- `h5` — exhibit and card titles

Visual treatment must follow semantic hierarchy rather than wrapper-specific exceptions.

## Vertical Rhythm

Every major section follows a repeated sequence:

1. Label
2. Display
3. Deck
4. Body, when needed
5. Content

Spacing is controlled by a small shared scale. New components should not introduce unique margin systems unless the content model genuinely requires one.


## Layout Owns Width

Component layout determines available width.

Typography rules define appearance, not column geometry.

Do not use character-based `max-width`, fixed text widths, or wrapper-specific width overrides to force line breaks when an adjacent artifact determines the available space.

For sections pairing narrative content with a Field Note or Exhibit:

1. Define an explicit grid
2. Give the narrative column `minmax(0, 1fr)`
3. Give the artifact a deliberate fixed or bounded width
4. Let headings and paragraphs use the full narrative column
5. Move full-width evidence below the introductory grid


## Decorative Artifacts Must Not Dictate Narrative Measure

A Field Note may accompany a section without becoming a structural column.

When an artifact occupies unused visual space rather than participating in the reading flow, position it independently and let the narrative use the full available measure.

Reserve a grid column only when both columns are genuinely part of the same reading structure.


## Shared Editorial Hierarchy

All major sections use the same visual order:

1. Label
2. Major section thesis
3. Explanatory copy
4. Major subsection thesis, when needed
5. Shared bold title
6. Supporting evidence or body copy

### Shared bold title

Questions, principles, capability names, card titles, publication titles, and timeline titles use one shared token.

They must share:

- font family
- size
- weight
- line height
- letter spacing
- color

Component-specific selectors may control spacing, but must not redefine the typography.


## Current Typography Hierarchy

### Hero

The hero is locked to the approved index 5 composition.

Do not alter its width, scale, wrapping, grid proportions, or operating-model placement unless the change is explicitly requested.

### Philosophy

Philosophy is also treated as an approved baseline.

Its thesis, narrative, Field Note, and three principles should not inherit later section-level overrides.

### Systems

Systems is the hero-level section for the Learn → Align → Decide structure.

Each subsection begins with:

1. blue uppercase label
2. italic serif leadership statement
3. sans-serif explanatory copy
4. supporting capabilities and exhibits

Approved leadership statements:

- *Strengthening organizational learning.*
- *Create confidence across people, priorities, and products.*
- *Improve decision quality under uncertainty.*

The wording is intentional. Each statement describes something Bryanne does as a leader and should not be rewritten merely to create grammatical parallelism.

## Field Note Rules

Field Notes function as annotations.

They should not include:

- external “Annotation” labels
- blue leader lines
- decorative callout text outside the note

Placement rules:

- Field Note 01 accompanies Philosophy
- Field Note 02 remains within the Systems introduction and may later be replaced by an image
- Field Note 03 accompanies Learn
- Field Note 04 belongs beside the Align heading
- later Field Notes should remain close to the section idea they interpret

A Field Note should never reserve unnecessary width for unrelated copy or overlap readable content.

## Navigation Binder Clip

Only one moving binder clip may appear in the navigation.

The clip is represented by the `.nav-clip` element.

Navigation-link pseudo-elements must not render additional binder images.

## Flagship Principle Cards

The three Design With Us cards are the strongest card treatment on the site:

- Memory
- Infrastructure
- Strategy

Their blue labels align at the same vertical position.

Their serif titles should remain prominent but fully contained within the card at supported desktop widths.

Supporting cards should remain visually quieter.

## Spacing Tokens

Use shared spacing tokens for rhythm:

- section
- chapter
- block
- paragraph
- tight

Spacing should support reading order and hierarchy rather than create decorative emptiness.
