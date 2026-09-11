# Repository Guidelines

## Project Structure & Module Organization

Corsair combines a tabletop RPG rulebook with a Java rules simulator.
- `src/main/java/org/pcsiszar/corsair/`: mechanics organized into `character`, `combat`, `dice`, `test`, and `track` packages. The production `test` package models in-game tests.
- `src/test/java/org/pcsiszar/corsair/`: JUnit tests and probability simulations.
- `rulebook/Rulebook.md`: rulebook entry point; topic folders contain rules, classes, equipment, lore, and GM guidance.
- `rulebook/**/*_Sheet.html`: printable character, class, equipment, and reference sheets.
- `.agents/skills/`: specialist guidance for rules, lore, writing, equipment, classes, and printable sheets.

## Build, Test, and Development Commands

Install JDK 21 and Maven; no Maven wrapper is checked in. Run commands from the repository root:
- `mvn compile`: compile the Java implementation.
- `mvn test`: run tests, including Monte Carlo simulations.
- `mvn "-Dtest=DieTest,ComplexTestTest" test`: run focused mechanics tests.
- `mvn "-Dtest=MonteCarloTest" test`: generate probability simulation output.
- `mvn package`: test and package the project under `target/`.

The POM does not configure an application launcher. Preview Markdown and open HTML sheets in a browser; inspect A4 print preview for layout changes.

## Coding Style & Naming Conventions

Follow existing Java style: two-space indentation, same-line opening braces, `PascalCase` classes, `camelCase` methods and fields, and `UPPER_SNAKE_CASE` constants. Keep packages under `org.pcsiszar.corsair`. Lombok is available; follow nearby usage. No formatter or linter is configured in `pom.xml`.

Use descriptive rulebook filenames with underscores, such as `Ship_Rules.md`, and matching `Name_Sheet.html` names for sheets. Preserve relative links and established game terminology.

## Testing Guidelines

Use JUnit Jupiter 5. Name test classes `*Test` and methods descriptively, following existing `testSuccessfulComplexTest` examples. Prefer deterministic `TestDie` rolls for mechanics assertions. Monte Carlo output supports balance analysis but does not replace assertions. No coverage threshold is configured; verify Maven actually discovers and executes tests.

## Commit & Pull Request Guidelines

Recent commits use imperative summaries such as `Add`, `Revise`, and `Overhaul`; scoped prefixes such as `feat(classes):` also appear. Keep commits focused. In pull requests, explain the affected behavior or rules, include validation results, link relevant issues, and provide screenshots or print previews for sheet changes. Keep related rules and sheets consistent.
