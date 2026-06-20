# COIN / ICS Game Designer

A [Claude](https://claude.com) skill for designing board games in the **COIN** (Counter-Insurgency) and **ICS** (Irregular Conflict Series) tradition — asymmetric conflict simulations where 1–4 factions with fundamentally different capabilities, resources, and victory conditions compete to shape the outcome of an irregular conflict.

The skill encodes the structural and mechanical conventions of the COIN system — eligibility tracks, operations and special activities, event cards, propaganda/winter rounds, faction archetypes, and victory conditions — so it can take a historical conflict or theme and produce a coherent game design.

## What it does

Given a conflict or theme, the skill works from research and faction modeling through to mechanics, producing a structured design document covering:

- **Factions** — 2, 3, or 4 asymmetric factions with distinct capabilities, resources, and victory conditions
- **Operations and special activities** — each faction's menu of actions and how they pair
- **Eligibility / initiative structure** — the classic 4-player cylinder, the 3-player every-turn format, or the 2-player Initiative Track
- **Event decks** — card-assisted play with sample event cards
- **Map and population** — geography plus support/opposition as the contested resource
- **Propaganda / winter rounds** — victory checks, resource income, attrition, and political shifts

It supports 2-player ([Colonial Twilight](https://boardgamegeek.com/boardgame/207894/colonial-twilight) style), 3-player (People Power / All Bridges Burning style), and 4-player (the classic Andean Abyss / Fire in the Lake format) designs.

## Background

The COIN system was created by Volko Ruhnke and published by [GMT Games](https://www.gmtgames.com/). It models conflicts where the sides aren't symmetric armies but governments, insurgents, warlords, foreign powers, and political movements, each operating by different logic.

## Repository layout

- `SKILL.md` — the skill definition and design knowledge
- `evals/evals.json` — evaluation prompts for the skill
- `eval_review.html` — eval review viewer
- `references/` — supporting reference material

## Usage

Install `SKILL.md` as a Claude skill, then ask Claude to design a COIN/ICS game — for example:

> Design a 4-player COIN game about the Troubles in Northern Ireland, covering roughly 1969–1998.

## License

BSD 3-Clause. See [LICENSE](LICENSE).
