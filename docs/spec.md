# Airbnb React/JSX style — throughline source

This document is **generated from the graph** by `tl docs`; `tl docs --check` gates it in CI. The prose headings are hand-owned — everything between `tl:*` markers is injected from the YAML items, so the published spec can never drift from the graph.

This source re-expresses the **Airbnb React/JSX Style Guide** as a grounded IDD graph: each major section is a `user_requirement`, and every individual rule is a `system_requirement` that `implements` its section. The guide reference lives in `attrs.source_ref`; the throughline UIDs are this source's own and immutable — a consumer cites a rule as `react:SR-0001`, never by section name.

It carries
<!-- tl:count type == 'user_requirement' -->
15
<!-- tl:end --> sections and
<!-- tl:count type == 'system_requirement' -->
36
<!-- tl:end --> style rules.

## Purpose

<!-- tl:item INT-0001 -->
**INT-0001 — React components are written in one consistent, idiomatic JSX style** — `intent`, status `approved`

> The Airbnb React/JSX Style Guide exists so that React components across a large codebase read as though written by one author: consistent component structure, naming, declaration, alignment, spacing and prop conventions, favouring idiomatic JSX and modern React so that any engineer can read and change component code they did not write.

**source_ref**: Airbnb React/JSX Style Guide
<!-- tl:end -->

## Basic Rules

<!-- tl:item UR-0001 -->
**UR-0001 — Basic Rules** — `user_requirement`, status `approved`

> Rules governing how many components a file holds and whether JSX is used.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Basic Rules
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Basic Rules') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0001 | system_requirement | approved | Include only one React component per file |
| SR-0002 | system_requirement | approved | Always use JSX syntax |
<!-- tl:end -->

## Class vs Function Components

<!-- tl:item UR-0002 -->
**UR-0002 — Class vs Function Components** — `user_requirement`, status `approved`

> Rules governing when to write a class component and when to write a function component.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Class vs Function Components
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Class vs Function Components') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0003 | system_requirement | approved | Prefer function components |
| SR-0004 | system_requirement | approved | Do not use createReactClass |
<!-- tl:end -->

## Mixins

<!-- tl:item UR-0003 -->
**UR-0003 — Mixins** — `user_requirement`, status `approved`

> Rules governing the use of mixins.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Mixins
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Mixins') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0005 | system_requirement | approved | Do not use mixins |
<!-- tl:end -->

## Naming

<!-- tl:item UR-0004 -->
**UR-0004 — Naming** — `user_requirement`, status `approved`

> Rules governing filenames, reference names, component names and prop names.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Naming
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Naming') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0006 | system_requirement | approved | Use the jsx extension for components |
| SR-0007 | system_requirement | approved | Use PascalCase for filenames |
| SR-0008 | system_requirement | approved | Use PascalCase for components and camelCase for instances |
| SR-0009 | system_requirement | approved | Name a component after its file |
| SR-0010 | system_requirement | approved | Base a higher-order component displayName on both names |
| SR-0011 | system_requirement | approved | Do not reuse DOM prop names for other purposes |
<!-- tl:end -->

## Declaration

<!-- tl:item UR-0005 -->
**UR-0005 — Declaration** — `user_requirement`, status `approved`

> Rules governing how a component is declared and named.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Declaration
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Declaration') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0012 | system_requirement | approved | Name components by reference, not displayName |
<!-- tl:end -->

## Alignment

<!-- tl:item UR-0006 -->
**UR-0006 — Alignment** — `user_requirement`, status `approved`

> Rules governing the alignment of JSX syntax.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Alignment
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Alignment') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0013 | system_requirement | approved | Follow the JSX alignment style |
| SR-0014 | system_requirement | approved | Keep single-line JSX on one line |
<!-- tl:end -->

## Quotes

<!-- tl:item UR-0007 -->
**UR-0007 — Quotes** — `user_requirement`, status `approved`

> Rules governing quotation marks in JSX and in JavaScript.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Quotes
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Quotes') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0015 | system_requirement | approved | Use double quotes for JSX attributes |
<!-- tl:end -->

## Spacing

<!-- tl:item UR-0008 -->
**UR-0008 — Spacing** — `user_requirement`, status `approved`

> Rules governing whitespace in tags and in curly braces.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Spacing
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Spacing') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0016 | system_requirement | approved | Include one space in a self-closing tag |
| SR-0017 | system_requirement | approved | Do not pad JSX curly braces with spaces |
<!-- tl:end -->

## Props

<!-- tl:item UR-0009 -->
**UR-0009 — Props** — `user_requirement`, status `approved`

> Rules governing prop naming, prop values, accessibility props and prop spreading.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Props
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Props') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0018 | system_requirement | approved | Use camelCase for prop names |
| SR-0019 | system_requirement | approved | Omit the value of a true prop |
| SR-0020 | system_requirement | approved | Always include an alt prop on images |
| SR-0021 | system_requirement | approved | Do not use image words in alt text |
| SR-0022 | system_requirement | approved | Use only valid ARIA roles |
| SR-0023 | system_requirement | approved | Do not use accessKey |
| SR-0024 | system_requirement | approved | Avoid using array index as a key |
| SR-0025 | system_requirement | approved | Use props spread sparingly |
<!-- tl:end -->

## Refs

<!-- tl:item UR-0010 -->
**UR-0010 — Refs** — `user_requirement`, status `approved`

> Rules governing how refs are obtained.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Refs
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Refs') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0026 | system_requirement | approved | Use ref callbacks, not string refs |
<!-- tl:end -->

## Parentheses

<!-- tl:item UR-0011 -->
**UR-0011 — Parentheses** — `user_requirement`, status `approved`

> Rules governing parentheses around multiline JSX.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Parentheses
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Parentheses') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0027 | system_requirement | approved | Wrap multiline JSX in parentheses |
<!-- tl:end -->

## Tags

<!-- tl:item UR-0012 -->
**UR-0012 — Tags** — `user_requirement`, status `approved`

> Rules governing self-closing tags and closing-tag placement.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Tags
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Tags') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0028 | system_requirement | approved | Self-close tags with no children |
| SR-0029 | system_requirement | approved | Close a multiline tag on a new line |
<!-- tl:end -->

## Methods

<!-- tl:item UR-0013 -->
**UR-0013 — Methods** — `user_requirement`, status `approved`

> Rules governing event handlers, method binding, naming and render return values.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Methods
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Methods') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0030 | system_requirement | approved | Use arrow functions to close over local variables |
| SR-0031 | system_requirement | approved | Bind event handlers in the constructor |
| SR-0032 | system_requirement | approved | Do not underscore-prefix internal methods |
| SR-0033 | system_requirement | approved | Return a value from render methods |
<!-- tl:end -->

## Ordering

<!-- tl:item UR-0014 -->
**UR-0014 — Ordering** — `user_requirement`, status `approved`

> Rules governing the ordering of members within a component.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: Ordering
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: Ordering') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0034 | system_requirement | approved | Order class component members consistently |
| SR-0035 | system_requirement | approved | Declare propTypes, defaultProps and state as class fields |
<!-- tl:end -->

## isMounted

<!-- tl:item UR-0015 -->
**UR-0015 — isMounted** — `user_requirement`, status `approved`

> Rules governing the deprecated isMounted anti-pattern.

*Derives from:* INT-0001

**source_ref**: Airbnb React/JSX Style Guide: isMounted
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Airbnb React/JSX Style Guide: isMounted') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0036 | system_requirement | approved | Do not use isMounted |
<!-- tl:end -->

