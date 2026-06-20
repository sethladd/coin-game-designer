---
name: coin-game-designer
description: >
  Design COIN (Counter-Insurgency) and ICS (Irregular Conflict Series) board games with deep knowledge
  of the system's conventions: eligibility tracks, operations and special activities, event cards,
  propaganda/winter rounds, faction archetypes, and victory conditions. Use this skill whenever the user
  wants to design a COIN-style game, create factions for an irregular warfare game, develop event decks
  for asymmetric conflict simulations, or adapt a historical conflict into the COIN/ICS framework. Also
  trigger when the user mentions COIN series, GMT Games COIN, Volko Ruhnke, irregular conflict simulation,
  counterinsurgency game design, or wants to create an asymmetric wargame with an eligibility-based
  turn structure. Even if the user just names a historical insurgency or irregular conflict and asks for
  a game design, this skill is likely the right fit.
---

# COIN / ICS Game Designer

Design board games in the COIN (Counter-Insurgency) and ICS (Irregular Conflict Series) tradition — asymmetric conflict simulations where 1-4 factions with fundamentally different capabilities, resources, and victory conditions compete to shape the outcome of an irregular conflict.

This skill focuses on the *structural* and *mechanical* knowledge specific to COIN/ICS design. For broader game design philosophy (emergent narrative, theme-mechanic integration, player interaction theory), consult the `strategy-board-game-designer` skill. For writing the actual rulebook once the design is complete, use `board-game-rules-author`. For stress-testing the rules, use `board-game-logic-analyzer`.

## Player Count: 2, 3, and 4-Player Designs

COIN/ICS games work at 2, 3, or 4 players. The design considerations differ significantly by count:

**4-player (the classic COIN format).** Four factions with a card-driven eligibility system where only 2 of 4 factions act per card. Creates a web of shifting alliances and competing interests. Most published COIN games target this format (Andean Abyss, Fire in the Lake, A Distant Plain).

**3-player (the People Power / All Bridges Burning format).** Three factions, each eligible every turn rather than rotating 2-per-card. All factions get at least one action per turn, keeping all players engaged. People Power and Vijayanagara use this structure. Good for conflicts with three natural sides (e.g., Reds/Whites/Moderates in the Finnish Civil War).

**2-player (the Colonial Twilight format).** Colonial Twilight pioneered the 2-player COIN design using an **Initiative Track** instead of the 4-player eligibility cylinder:
- Initiative swings between players based on action strength: weaker actions preserve initiative, stronger actions forfeit it to your opponent
- The second player's eligible spaces may be constrained to areas adjacent to the first player's chosen space (speeds up decisions)
- Games tend to be shorter and more accessible (90-120 minutes vs. 4-6 hours)

When the user specifies a player count, design for that count from the ground up. When they don't, default to 4-player but note how the design could adapt. Some conflicts naturally suit one count: a bipolar conflict like the Algerian War fits 2 players; a three-way civil war fits 3; a multi-faction insurgency fits 4.

## What Makes COIN Games Distinctive

COIN games model conflicts where the sides aren't symmetric armies — they're governments, insurgents, warlords, foreign powers, criminal networks, and political movements, each operating by different logic. The system — created by Volko Ruhnke, a former CIA analyst specializing in insurgency — captures this through several interlocking innovations:

**Card-assisted (not card-driven) play.** This distinction matters. In card-driven games (CDGs), players spend cards for either operation points or events. In COIN, event cards serve as an additional dimension — they determine turn order and offer event options, but players choose their actions independently. Events don't cost resources to enact. Both the current card and the next card are always visible, enabling strategic planning.

**Eligibility-based initiative.** Rather than "I go, you go," factions take turns based on an eligibility track driven by event cards. Only 2 of 4 factions act per card. Acting now means you're ineligible next card. This models the reactive, opportunistic nature of irregular conflict.

**Operations + Special Activities.** Each faction has a menu of operations (march, train, rally, attack) and special activities (assassinate, govern, infiltrate, extort). The pairing of an operation with a special activity on a single turn is the core decision space. Special activities are restricted as to which operations they can accompany.

**Underground vs. Active piece states.** Insurgent guerrillas exist in two states: **Underground** (hidden, protected from most enemy action, but must activate to attack) and **Active** (visible, vulnerable, but tactically useful). This dual state creates fog of war — the government knows guerrillas are somewhere but not exactly where. Guerrillas must come out of hiding to fight, creating risk/reward decisions.

**Population as terrain.** The map isn't just geography — it's people. Support and Opposition among the population are the central contested resource. Having military control of a space is a *prerequisite* to influencing support, but it's the support/opposition alignment that determines victory.

**Propaganda/Winter rounds.** Periodically, the game pauses for a "state of the world" assessment — victory checks, resource income (the *only* time factions generate resources), attrition, political shifts. Resources are generated *only* during propaganda rounds, making them critical strategic inflection points.

## Design Process: From Conflict to Game

When a user provides a conflict or theme, work through these phases. Don't rush to mechanics — the research and faction-modeling phases determine whether the game will feel authentic.

### Phase 1: Conflict Research and Framing

Start by understanding the conflict deeply enough to identify the essential dynamics:

- **Who are the actors?** Not just the obvious two sides — COIN games shine when they capture 3-4 way tensions. In Vietnam, it's not just US vs. NVA; it's US vs. ARVN, NVA vs. VC, and the Saigon government vs. its own population.
- **What does each actor want?** Victory conditions reflect fundamentally different goals: the government wants stability, insurgents want to undermine legitimacy, foreign powers want influence, criminal networks want profit.
- **What's the time horizon?** COIN games span a specific period. The event deck paces the game through this period — longer conflicts need more cards or faster abstraction.
- **What's the geography?** The map captures strategic geography: population centers, remote bases, borders, key terrain, Lines of Communication. Not every city needs a space; only ones where meaningful decisions happen.
- **What makes this conflict *this* conflict?** Every irregular war has distinctive features — opium in Afghanistan, the Ho Chi Minh Trail in Vietnam, the Catholic Church in Latin American insurgencies. These become the game's mechanical signatures.

### Phase 2: Faction Design

COIN factions are the heart of the design.

#### Identity Triangle
Every faction sits at the intersection of:
1. **Strategic posture** — Occupier, incumbent government, guerrilla force, political movement, criminal enterprise, foreign intervener?
2. **Resource model** — Taxes, foreign aid, extortion, popular support, military hardware?
3. **Relationship to population** — Need popular support, coerce, ignore civilians, hide among them?

#### Faction Archetypes

**The Counterinsurgent Government (COIN faction).** Controls the state apparatus. Trains troops, builds institutions, conducts sweeps. Strong in conventional force but clumsy in population control. Wins by establishing support and legitimacy. Has more resources but less flexibility. Troops are always visible (Active).

**The Insurgent.** Operates through guerrillas who begin Underground (hidden). Rallies supporters, ambushes government forces, terrorizes or persuades the population. Hard to find when Underground, fragile when Active. Wins by spreading opposition or controlling territory through bases.

**The Foreign Power / Intervener.** Brings outside resources (troops, money, air power) but has limited patience. Often powerful militarily but struggles with legitimacy. Has a **Commitment track** that forces withdrawal if eroded — a faction-specific loss condition (as in A Distant Plain's Coalition).

**The Warlord / Criminal Network.** Motivated by profit or local power. Thrives on instability. Extracts resources and plays other factions against each other. Wins by accumulating wealth or controlling economic nodes. Often has unique economic mechanics (cultivation, trafficking).

**The Nonviolent Movement (Gandhi innovation).** Wins through protest, civil disobedience, and political organizing rather than violence. Uses Activists (immune to military action until they Protest), Non-Cooperation (disrupts Lines of Communication), and Demonstrations. Gandhi and People Power pioneered this archetype — it dramatically expands what COIN can model.

#### Faction Interaction Matrix
After defining factions, map their relationships:
- Which pairs are natural enemies?
- Which might temporarily ally?
- Where do their victory conditions inherently conflict?
- Where might one faction's success accidentally help another?
- Can any faction serve as "kingmaker" or balance-tipper?

The richest COIN games have factions where alliances shift. The government and foreign power are nominally allied but want different things. The insurgent and criminal network cooperate tactically but have incompatible end goals. All Bridges Burning adds a shared loss condition (foreign intervention) that forces all factions to cooperate against a common threat even while competing.

### Phase 3: Core Mechanics

#### The Eligibility System (4-Player Standard)

The 4-player COIN eligibility system works step by step:

1. **Two cards always visible.** The current event card is active; the next card is face-up so players can plan ahead.
2. **Faction symbols on the card** determine eligibility order (read left to right).
3. **Only 2 of 4 factions act per card.** The 1st Eligible faction chooses first, then the 2nd Eligible.
4. **Each acting faction chooses one of four options:**
   - **Execute the Event** — Take either the unshaded OR shaded text of the current event card (the executing faction chooses which interpretation, regardless of their faction type)
   - **Operation + Special Activity** — Conduct a full operation across multiple spaces, paired with one special activity
   - **Limited Operation** — Conduct an operation in a single space only, with no special activity (less powerful but cheaper)
   - **Pass** — Take no action; gain a small resource bonus; remain eligible for the next card
5. **The 1st Eligible's choice constrains the 2nd Eligible's options.** The Sequence of Play board shows which action pairs are available — the 2nd faction can only choose from the remaining adjacent option spaces.
6. **Factions that act become ineligible for the next card.** Factions that pass remain eligible.
7. **Eligibility resets at propaganda rounds** — all factions become eligible again.

**Frequency of action:** With 6-11 cards between propaganda rounds, a faction typically acts 3-4 times per period. Managing eligibility (when to act vs. when to pass) is a core strategic skill.

**Initiative preservation:** In some designs, choosing weaker actions (Limited Operation, Pass) preserves initiative (acting first next turn), while powerful actions (Operation + Special Activity) forfeit initiative. This creates a push-pull between doing more now vs. controlling when you act later.

#### The Eligibility System (2-Player: Initiative Track)

Colonial Twilight's 2-player system replaces the cylinder with an **Initiative Track**:
- The event card determines which faction has initiative (first choice)
- First player chooses: Event OR Operation + Special Activity
- Second player gets the remaining option OR a Limited Operation
- Choosing powerful actions ("shaded" side of the track) forfeits initiative to your opponent next turn
- Choosing restrained actions ("unshaded" side) preserves initiative
- This creates genuine tension: act powerfully now and lose control of timing, or act moderately and keep the tempo

#### The Eligibility System (3-Player)

People Power and Vijayanagara use a 3-player variant:
- All three factions are eligible every turn (no rotating ineligibility)
- Each faction gets at least one action per turn
- Event cards still determine turn order
- Keeps all players engaged throughout the game

#### Operations

Each faction gets 3-5 operations. These cover similar strategic needs but feel fundamentally different between factions:

| Strategic Need | Government Example | Insurgent Example |
|---|---|---|
| Move forces | **Sweep** (move + reveal Underground guerrillas) | **March** (move guerrillas, stay Underground) |
| Build strength | **Train** (place troops/police/bases) | **Rally** (place guerrillas/bases, go Underground) |
| Attack | **Assault** (remove enemy pieces using Active forces) | **Ambush** (attack from Underground, then may go Active) |
| Influence population | **Civic Action** (shift toward Support) | **Agitate/Terror** (shift toward Opposition) |
| Gather resources | **Govern** (collect taxes from controlled areas) | **Extort** (collect money, may expose you) |

**Key principle:** Operations reflect *how* each faction fights. A government Sweep reveals hidden enemies. An insurgent March keeps forces Underground. Same strategic purpose (repositioning), completely different tactical experience.

**Operations cost resources** and can target multiple spaces (1 resource per space for a full Operation). Limited Operations target a single space and are cheaper or free.

#### Special Activities

Each faction gets 2-4 special activities — unique capabilities that define their character. Special activities are paired with Operations (executed immediately before, during, or after an Operation) and many are restricted to specific Operation types:

- **Government:** Eradicate (destroy resources/crops), Govern (collect taxes, build legitimacy), Surge (emergency reinforcements), Civic Action
- **Insurgent:** Assassinate (remove specific targets), Infiltrate (place Underground pieces), Extort (collect money from population), Ambush (attack from hiding)
- **Foreign Power:** Air Strike (ranged attack, may accompany Sweep/Assault only), Aid (fund allied faction), Advise (boost ally effectiveness)
- **Criminal Network:** Bribe (flip enemy units), Traffic (move contraband for profit), Cultivate (plant crops for future income), Launder (convert resources to influence)

**Design principle:** Special activities are where the game's personality lives. They create memorable moments and tough decisions. The restriction on which operations they can accompany prevents overpowered combos while encouraging diverse play.

#### Underground vs. Active Piece States

This is a fundamental COIN mechanic that creates fog of war:

**Underground guerrillas:**
- Hidden from the enemy (represented by pieces placed face-down or with a hidden marker)
- Protected from most enemy operations — government must Sweep to reveal them before Assaulting
- Required for certain operations: Terror, Ambush, and other stealth-dependent actions typically require at least 1 Underground guerrilla
- Cannot attack or project force while Underground (must activate first)

**Active guerrillas:**
- Visible on the board, exposed to enemy action
- Can participate in attacks and hold territory
- Removed first when casualties occur (Underground pieces are preserved as higher-value assets)

**Piece state transitions:**
- Rally typically places guerrillas Underground (they start hidden)
- Attacking or conducting Terror flips guerrillas to Active (they're exposed by acting)
- Some operations allow guerrillas to go back Underground (hiding after an ambush)
- Government Sweep operations reveal (flip) Underground guerrillas to Active, making them vulnerable to Assault

**Design implication:** This creates a cat-and-mouse dynamic where insurgents build strength in hiding and must choose when to reveal themselves. The government invests in intelligence and sweep operations to find hidden enemies before they strike.

#### The Event Deck

The event deck is the game's narrative spine. COIN uses a **card-assisted** system (not card-driven — an important distinction):

**Card anatomy:**
- **Faction symbols at top** — Determine eligibility order for this turn (read left to right)
- **Card number** — Determines position in the deck
- **Event title** — A historical event or development
- **Italicized flavor text** — Historical context (no mechanical effect)
- **Unshaded event text** — One interpretation of the event, often (but not always) favoring COIN factions
- **Shaded event text** — Alternative interpretation, often favoring insurgent factions

**Critical rule:** The executing faction may choose *either* the unshaded or shaded text, regardless of which faction they are. The labels suggest typical allegiances but don't restrict choice — a government player might choose the shaded text if it helps them in the current situation.

**Deck structure:**
- Decks contain 36-72 event cards depending on the game
- The deck is divided into **segments** (typically 3-4 piles of cards)
- One Propaganda/Winter card is shuffled into each segment
- Propaganda cards are placed in the lower portion of each pile to prevent them from appearing too early
- This structure ensures roughly even pacing while maintaining uncertainty about exactly when propaganda will hit

**Pivotal Events (advanced variant from Fire in the Lake):**
Some games include **Pivotal Event** cards — faction-specific events held face-up outside the main deck. A faction can interrupt the normal sequence to play their Pivotal Event when conditions are met, representing historical turning points (Tet Offensive, Vietnamization, Easter Offensive). These are optional and add drama but complexity.

**Capability cards:** Some events grant permanent or lasting bonuses (Capabilities) rather than one-time effects. These stay in play and modify the rules for the rest of the game, representing lasting shifts in the conflict.

**Event design principles:**
- Events represent "opposed effects of the same cause, forks in the historical road, or instances subject to interpretation"
- The best events create genuine dilemmas: powerful enough that factions will sacrifice their Operation just to execute (or deny) them
- Events should matter differently depending on the current game state
- Some events should be powerful enough to swing the game — these create narrative climax moments

#### Support, Opposition, and Control

The population alignment system is the political heart of COIN:

**Support/Opposition spectrum:** Each populated space tracks alignment on a 5-level scale:
- Active Support → Passive Support → Neutral → Passive Opposition → Active Opposition

**How alignment shifts:**
- Government operations (Civic Action, Govern) shift spaces toward Support
- Insurgent operations (Agitate, Terror) shift spaces toward Opposition
- Terror operations are fast but generate backlash; Civic Action is slow but durable
- Alignment shifts require military control first — you can't win hearts and minds in a space you don't hold

**Control calculation:**
- A faction **controls** a space when they have more pieces there than all other factions combined
- Important exception: enemy **bases** in a space prevent control even if you have numerical superiority in troops
- This means insurgents can deny government control by maintaining bases, even when outnumbered
- "COIN Control" requires government/counterinsurgent pieces exceeding all enemies; "Insurgent Control" requires the reverse

**Why this matters for victory:** Military control is a prerequisite to building Support or Opposition, but it's the Support/Opposition alignment that drives victory conditions. A government player who controls the board militarily but hasn't built Support is losing. An insurgent who has spread Opposition across many spaces is winning even without military dominance.

#### Lines of Communication (LOCs)

LOCs are a distinctive COIN map feature that many new designers underestimate:

**What they are:** Roads, railways, rivers, and trade routes connecting spaces on the map. They're not just borders — they're separate game features that can be controlled, sabotaged, patrolled, and fought over.

**Mechanical functions:**
- Government patrols along LOCs to secure them (placing troops on the LOC itself)
- Insurgents can sabotage LOCs (disrupting government resource collection and movement)
- Controlling LOCs generates economic resources during propaganda rounds
- Some factions can only move along LOCs (government convoys); others can move off-road (guerrillas through jungle/mountains)
- Non-Cooperation (in Gandhi) blocks LOCs through civil disobedience

**Design principle:** LOCs add a network-control dimension to area control. Instead of just "who controls which region," players also contest "who controls the connections between regions." This creates a more sophisticated map strategy and rewards positional play.

#### Propaganda / Winter / Coup Rounds

Different COIN games use different terminology for these periodic assessment rounds — Propaganda (Andean Abyss), Winter Quarters (Liberty or Death), Coup (A Distant Plain), Epoch — but the structure is similar:

**Step-by-step sequence:**

1. **Victory check** — Each faction checks their threshold condition. If met, that faction wins immediately. If multiple factions meet conditions, tiebreaker rules apply. If none, continue.

2. **Resource collection** — The *only* time factions generate resources. Each faction's formula is different:
   - Government: Resources based on total Support across controlled spaces
   - Insurgent: Resources based on total Opposition or number of bases
   - Foreign Power: Fixed allocation modified by Commitment track
   - Criminal: Resources from controlled economic zones, trade routes, cultivation
   - The amount collected directly determines capability in the next period

3. **Support/Opposition phase** — Population alignment may shift based on conditions:
   - Government may spend resources to shift spaces toward Support (every X resources = 1 shift)
   - Insurgent may shift spaces toward Opposition
   - Terror markers hamper Support-building (population doesn't trust a government that can't protect them)

4. **Attrition and redeploy** — Forces without supply may be removed. Pieces return to available pools. Temporary effects expire.

5. **Eligibility reset** — All factions become eligible again for the next card.

**Strategic weight:** Because resources are only generated during propaganda rounds, the entire game revolves around positioning for these checkpoints. Players must plan their resource expenditure to last between propaganda rounds while maximizing their position when the round arrives.

### Phase 4: Victory Conditions

COIN victory conditions are **threshold-based** (not cumulative VP), checked at propaganda rounds:

**Government:** Population support + control. "Total Support + COIN Control >= X"

**Insurgent:** Opposition + infrastructure. "Total Opposition + Insurgent Bases >= X"

**Foreign Power:** Patronage + manageable commitment. "Controlled spaces >= X while Commitment Track <= Y"

**Criminal Network:** Economic resources + operational freedom. "Total Resources + Open Spaces >= X"

**Nonviolent Movement (Gandhi model):** Political legitimacy + institutional presence. "Protest spaces + Support for independence >= X"

**Key design principles:**
- Victory conditions should be partially visible (other players can estimate how close you are to winning)
- Conditions should create tension between nominal allies (government wants support; foreign power wants low commitment — hard to achieve simultaneously)
- Some factions should be able to achieve conditions through different strategies
- Consider shared loss conditions (All Bridges Burning: foreign intervention triggers if any faction gets too extreme, causing all players to lose)

### Phase 5: Map Design

COIN maps encode strategic geography:

**Space types:**
- **Cities** — High population, connected by roads/LOCs, usually start under government control. Government operations are more effective here; insurgents are more exposed.
- **Provinces/Departments** — Rural areas with moderate population. Balanced terrain for both sides.
- **Jungle/Mountain/Remote** — Difficult terrain favoring guerrillas. Government Sweep operations cost double here. Insurgent Rally and March are cheaper or free. Key for insurgent bases.
- **Lines of Communication (LOCs)** — Roads and routes *between* spaces, treated as separate features that can be patrolled, sabotaged, and fought over. Control them for economic income and movement.
- **Borders/Off-map connections** — Where foreign support enters, refugees flee, smuggling occurs. May connect to off-map havens (like the Border Haven mechanic in A Distant Plain).

**Map design principles:**
- Population distribution drives strategy — factions compete for populated spaces, but bases hide in remote ones
- Terrain gives asymmetric advantages: mountains favor guerrillas, cities favor police, LOCs favor government logistics
- Typical COIN maps have 20-30 spaces (Andean Abyss: 27 regions; Fire in the Lake: 30 provinces/cities)
- Economic nodes (ports, resources, trade routes) give the criminal/economic faction its geography
- Each space should present interesting decisions — if a space never matters, cut it

#### Bot / Non-Player System

All COIN games include bot sheets for solo and reduced-player-count play:

**How bots work:** Flowchart-based decision trees that monitor board state and select actions. The bot checks conditions ("Does this faction have X pieces available?", "Would this action produce Y result?") and follows if-then branches to select operations.

**Design considerations:** When designing a game, consider how each faction would behave as a bot. If a faction's strategy requires complex long-term planning or subtle diplomacy that's hard to automate, it may need simplification for bot play. Bots work best when factions have clear priorities and measurable board states to evaluate.

## Design Document Template

When producing a COIN game design document, organize it as follows:

```
# [Game Title]
## [Conflict], [Time Period]

### Overview
[2-3 paragraphs: What conflict does this model? What's the central tension?
What question does this game explore through play? Player count and estimated play time.]

### Factions
[For each faction:]
#### [Faction Name]
- **Role in conflict:** [historical role]
- **Strategic posture:** [archetype and variations]
- **Piece types:** [troops, guerrillas (Underground/Active), bases, special pieces]
- **Resources:** [what they track and manage]
- **Victory condition:** [specific threshold checked at propaganda rounds]
- **Operations:** [list with brief descriptions, noting which can be Limited Ops]
- **Special Activities:** [list with descriptions, noting which Operations they can accompany]
- **Starting position:** [pieces and placement]
- **Personality:** [how this faction *feels* to play]

### Faction Interaction Matrix
[Table or description of key faction relationships and tensions]

### The Map
[Description of spaces, connections, LOCs, terrain types, population distribution,
and economic geography. Note number of spaces and key strategic regions.]

### Sequence of Play
[The eligibility system (4p/3p/2p), the choice tree (Event / Op+SA / LimOp / Pass),
how eligibility/initiative flows between turns]

### Event Deck
[Deck structure: number of cards, segments, propaganda card placement.
5-10 sample event cards with BOTH unshaded and shaded text, historical context,
and eligibility order. Note any Pivotal Events or Capabilities.]

### Propaganda Round
[Step-by-step sequence: victory check, resource collection formulas per faction,
support/opposition phase, attrition, eligibility reset]

### Key Mechanics
[Mechanics unique to this game — the distinctive "hook" that makes this game
this game. Every COIN game needs at least one signature mechanic.]

### Design Notes
[Why decisions were made, historical compromises, closest published COIN game
as reference point, open playtest questions]
```

## Reference: Published COIN and ICS Games

These games establish the design vocabulary. When designing a new game, identify which existing game is closest in structure and use it as a reference point.

### Classic COIN Series (GMT Games)

**Andean Abyss** (2012, Volko Ruhnke) — The original. Colombia 1990s. Government, FARC, AUC, Cartels. 4 players, 27 regions. Established every core mechanic. Best reference for: drug trade economics, criminal faction design.

**Cuba Libre** (2013, Ruhnke & Trevino) — Cuban Revolution. Tighter and faster than Andean Abyss, only 3 major cities. GMT's recommended starter COIN game. Best reference for: accessible designs, compact maps, shorter play times.

**A Distant Plain** (2013, Ruhnke & Train) — Afghanistan. First COIN with two counterinsurgent factions that must coordinate (Coalition + Government). Introduces Patronage (corruption) mechanic. 72 event cards. Best reference for: foreign intervention dynamics, corruption, paired COIN factions.

**Fire in the Lake** (2014, Ruhnke & Herman) — Vietnam War. Most complex classic COIN. 8 troop types (vs. 5 in Andean Abyss), 30 provinces. Introduces **Pivotal Events** and the Trail mechanic for NVA supply. Best reference for: complex multi-front wars, supply line mechanics, air power.

**Liberty or Death** (2016, Harold Buchanan) — American Revolution. Winter Quarters (propaganda variant), French intervention, political dynamics alongside military. Propaganda cards sorted into lower third of each pile for better pacing. Best reference for: colonial-era conflicts, foreign alliance mechanics.

**Falling Sky** (2016, Volko & Andrew Ruhnke) — Caesar's Gallic Wars. Adapts COIN to ancient warfare. Shows how the system stretches beyond modern insurgency. Best reference for: pre-modern conflicts, tribal dynamics.

**Colonial Twilight** (2017, Brian Train) — Algerian War 1954-62. First 2-player-only COIN. **Initiative Track** instead of eligibility cylinder. Shows how to streamline without losing the soul of the system. Best reference for: 2-player design, bipolar conflicts, decolonization.

**Pendragon** (2017, Marc Gouyon-Rety) — Late Roman Britain. Stretches COIN into dark-age tribal dynamics. Introduces faction-specific Pivotal Events with unique triggering conditions. Best reference for: ancient/medieval settings, civilization collapse.

**Gandhi** (2019, Bruce Mansfield) — Indian Independence 1917-1947. Revolutionary: introduces the **Nonviolent faction type** — Activists immune to military action, Protest markers, Non-Cooperation blocking LOCs, Restraint Track measuring conflict severity. Best reference for: non-violent resistance, civil disobedience, political movements.

**All Bridges Burning** (2019, VPJ Arponen) — Finnish Civil War 1917-18. Three factions: Reds, Whites (Senate), Moderates. First COIN with a **shared loss condition** — if foreign intervention (German or Russian) gets too high, all players lose Finnish independence. Moderates have all actions available from game start; other factions unlock actions over time. Best reference for: 3-faction design, shared loss conditions, non-violent third faction.

**People Power** (2020, Gonzalo Santacruz) — Philippine People Power Revolution 1981-86. 3-player design where all factions act every turn. **Election Cycle** replaces propaganda rounds. **Acts of Desperation** deck adds hidden objectives for the revolutionary finale. Best reference for: 3-player sequence, election mechanics, revolution endgame.

### Irregular Conflict Series (ICS)

ICS games are **"model-first"** — they modify core COIN mechanics to fit their specific conflicts, sometimes radically. ICS represents an experimental branch with greater design freedom.

**Vijayanagara** (ICS, Leibert & Rathnam) — Deccan Empires of Medieval India 1290-1398. Three factions. **Completely removes Support/Opposition** — uses a Tributary Control System instead, where provinces are classified by their relationship to Delhi. Uses People Power's 3-player sequence. Best reference for: removing support/opposition, medieval settings, tributary systems.

**A Gest of Robin Hood** (ICS, Fred Serval) — Nottinghamshire. 2-player. Introduces **hidden movement** to the COIN framework (Robin hides among Merry Men; Sheriff must find him). Carriages on LOCs carry wealth and may conceal traps. 45-90 minutes, ages 12+. Best reference for: hidden movement, family-accessible design, radically streamlined COIN.

**Cross Bronx Expressway** (ICS, Non-Breaking Space) — South Bronx urban development 1940-2000. **Non-insurgency conflict entirely.** Three factions: Public, Private, Community stakeholders. **Collective loss condition** alongside competitive victory. Proves ICS can model stakeholder conflicts, not just warfare. Best reference for: non-military conflicts, cooperative-competitive hybrid.

**Echo from the Dark** (ICS, Adam Blinkinsop) — Science fiction. **Most radical ICS departure.** Replaces event deck with **Technology deck** (factions research rather than respond to events). Every faction acts every turn (no eligibility rotation). 8 factions to choose from with modular selection. Best reference for: what happens when you push COIN mechanics to their limit.

### Key Designers and Their Contributions

**Volko Ruhnke** (creator) — Former CIA analyst. Design philosophy: asymmetric factions in ends, ways, and means; initiative matters more than firepower; population-centric strategy over territorial conquest.

**Brian Train** — A Distant Plain, Colonial Twilight, China's War. Specialist in streamlined COIN design and 2-player adaptation. 20+ years designing conflict simulations.

**Harold Buchanan** — Liberty or Death. Refined propaganda card pacing (sorted into lower third of piles).

**Bruce Mansfield** — Gandhi. Revolutionized COIN by proving it can model nonviolent resistance.

## Common Design Pitfalls

**Symmetric insurgents.** If your insurgent factions feel interchangeable, their operations and special activities aren't differentiated enough. Each faction should fight *differently*, not just in a different color.

**Ignoring Underground/Active states.** The dual piece state is fundamental to COIN's fog of war. If you design insurgent pieces without Underground/Active distinction, you lose the cat-and-mouse dynamic that makes the system work.

**Making COIN a card-driven game by accident.** COIN is card-*assisted*. If your events cost operation points to execute, or if players draw cards into a hand to play, you've designed a CDG, not a COIN game. Events are resolved alongside the card-driven turn order, not instead of actions.

**Toothless propaganda rounds.** If nothing dramatic happens during propaganda, the game loses its rhythm. Propaganda should feel like a reckoning — and since it's the only time resources generate, it should have real teeth.

**Event cards as flavor text.** Events that don't meaningfully alter the game state are wasted cardboard. Every event should present a real decision — powerful enough that factions will sacrifice their Operation to execute (or deny) the event.

**LOCs as decoration.** If Lines of Communication are just borders between spaces, you're missing a design opportunity. LOCs should be separate features that can be patrolled, sabotaged, and fought over.

**Victory conditions that don't create tension between allies.** If the government and foreign power can both win simultaneously without friction, you're missing the best part of COIN design — the alliance that slowly fractures.

**Overcomplicated special activities.** If a special activity requires a paragraph to explain, simplify it. COIN's elegance comes from simple operations that interact in complex ways.

**Forgetting that resources only generate at propaganda.** If you let factions generate resources every turn, you've eliminated one of COIN's core resource-tension mechanics. The scarcity between propaganda rounds is what makes every action feel consequential.
