Root: [[Fundamentals of Level Design]]
###### Tag: #OnlineCourse #Coursera 
###### Created on: [[Jun 24, Tuesday, 2025]]
###### Last Modified: [[Jun 25, Wednesday, 2025]]
---
# Level Design Document: Medieval Village Prototype

# **Concept**

## Requirements

*   The level must feature a central **Castle Area** with a main castle building and surrounding structures, visually distinct and defensible.
*   The level must include an adjacent **Village Area** with a medieval architectural style, containing multiple **Villager Homes**.
*   The village must feature a functional **Farming Area** with diverse crop representations and an **Animal Farm** area (e.g., for cows, pigs, or goats).
*   The village must include key structures such as a **Smithy**, a **Tavern**, and a **Village Market** area.
*   The gameplay perspective must be **Third-Person**.
*   The level must support a **Day/Night Cycle** that influences NPC behavior and gameplay opportunities (e.g., stealth).
*   Player interaction with the environment must include the ability to **open doors and chests**.
*   The design must accommodate **stealth gameplay**, including areas for hiding (bushes, shadows) and paths for sneaking.
*   The design must allow for two distinct player approaches/paths:
    *   **Thievery/Stealth Path:** Involving lockpicking (conceptual), sneaking past/incapacitating guards, and looting.
    *   **Questing/Hero Path:** Involving interaction with key NPCs (e.g., Lord of the Castle) for missions.
*   NPC presence will be represented by **static placeholder dummies** in the greybox phase, indicating intended roles and locations.

## Goals

*   The player should feel a sense of a living, albeit simplified, medieval settlement.
*   The layout should encourage exploration and discovery of different zones and potential secrets.
*   The level design should clearly afford different gameplay styles (direct engagement vs. stealth).
*   The visual distinction between the Castle, Village, and Farming areas should be clear even in greybox form.
*   The level should provide a sense of progression or varied opportunities depending on the time of day.

## Game Context

*   This level serves as a self-contained prototype demonstrating core open-world style level design principles for a single-player experience.
*   It is designed as a capstone project for the "Fundamentals of Level Design" course.
*   It introduces foundational mechanics such as exploration, environmental interaction, and the spatial requirements for stealth and NPC-driven quest systems.

## Setting

*   The level is set in a small, relatively isolated **medieval European-style village** built around a local Lord's castle.
*   **Castle Area:** Constructed primarily of stone, featuring a main keep, courtyards, defensive walls (traversable), and potentially some auxiliary buildings within its compound.
*   **Village Area:** Composed of timber-framed buildings with wattle-and-daub or stone infill, thatched or shingle roofs. Includes residential homes, a smithy (with forge area), a tavern (possibly with a common room and some private rooms), a market square with stall placeholders, and a water well.
*   **Farming Area:** Open fields sectioned for different crops, and an enclosed area for animal husbandry.
*   **Overall Atmosphere:** Aims for a classic medieval fantasy feel. Lighting will be crucial, with brighter, more open lighting during the day, and more shadowed, atmospheric lighting at night to support stealth.
*   **Asset Style (Conceptual for Greybox):** While using primitives and SuperGrid, the forms should suggest materials like wood, stone, thatch, and dirt paths.

## Time

*   The level operates on a full **Day/Night Cycle**.
*   The implied season is temperate, such as late spring or summer, to justify active farming.

# **Metrics**

## Player and player movement

*   Utilizes the standard third-person character controller from the UE Animation Sample project.
*   Movement speeds: Standard walk, run, jump, crouch.
*   Interaction radius for doors, chests, (placeholder) NPCs: Approximately 1.5 - 2.5 meters.
*   Player height: Approx. 1.8 meters (standard UE mannequin).
*   Jump height / distance: Standard UE Animation Sample values. Cover objects and climbable ledges (if any) to be designed around these.

## World

*   Gravity: Standard Earth-like gravity.
*   Scale: The village is designed to be explorable within a reasonable timeframe for a prototype.
    *   Castle Compound: Approx. 80m x 80m.
    *   Village Proper (excluding farms): Approx. 150m x 150m.
    *   Farming Area: Extends outwards from the village.
    *   Building heights: Villager homes 1-2 stories, Tavern/Smithy potentially larger, Castle Keep 3-4 stories. Wall heights designed to be significant obstacles yet potentially scalable in specific points or with tools (future scope).
*   Visibility: Clear sightlines in open areas, more restricted in dense village sections or forested peripheries.

## Items

*(Conceptual items the level design should support space for, not necessarily functional in greybox)*
*   **Lockpicks (Conceptual):** Represented by locked doors/chests.
*   **Quest Items (Conceptual):** Spaces for NPCs to give/receive items, or for items to be found in the world.
*   **Lootable Items (Conceptual):** Currency, valuables. Chests will be placed in interiors.
*   **Tools/Weapons (Conceptual):** Smithy designed to look like it produces these. Guard placeholders might imply weapon use.

# **Narrative & Drama**

## Beat Chart

*   **Arrival/Initial Exploration:** Player enters the village, gets a feel for the layout, and observes the different zones (Castle, Village, Farms). Low drama.
*   **Discovering Opportunity:** Player identifies potential interactions – a quest from an NPC placeholder (e.g., a note by a dummy Lord), or a vulnerable house to loot at night. Rising interest.
*   **First Challenge Attempt:**
    *   Path A (Hero): Player approaches the Castle to "interact" with the Lord placeholder.
    *   Path B (Thief): Player attempts to sneak past a guard placeholder or "lockpick" a door.
    *   This beat provides a small spike in tension/engagement.
*   **Exploration & Zone Discovery:** Player moves through distinct areas like the Tavern, Smithy, Farms, understanding their purpose. Ambient engagement.
*   **Day/Night Transition Impact:** Player observes changes (e.g., "activity" shifting, different guard patrols, locked doors), reinforcing gameplay choices.

## Explicit

*(Narrative elements that the level’s design and text/UI prompts would directly convey)*
*   Visual cues distinguishing different building functions (e.g., a forge for a smithy, beds for homes).
*   Placement of (placeholder) NPCs to clearly indicate roles (e.g., guard at a gate, farmer in a field, Lord in the castle keep).
*   Locked doors explicitly communicate a barrier requiring a specific action (lockpicking).
*   Signs or visual markers for key locations like "Tavern" or "Market."

## Implicit

*(Narrative elements suggested by the environment and layout)*
*   The size and defensibility of the castle imply the Lord's importance and potential threats.
*   The layout of the village (e.g., proximity of homes to farms, market to tavern) suggests daily life patterns.
*   Well-maintained areas might suggest prosperity, while run-down sections could imply neglect or poverty.
*   Hidden paths or secluded spots suggest opportunities for stealth or secret meetings.
*   Placement of guard posts and patrol routes imply areas of value or vulnerability.
# **Mapping**

## Landmarks

*   **Macro:** The Castle Keep (tallest structure, visible from most of the level), the main Windmill in the farming area (if applicable).
*   **Meso:** The central Village Well/Square, the Tavern building (distinctive architecture/signage placeholder), the Smithy (visible forge/chimney), the main entrance gate to the village, the bridge crossing into the farming area.
*   **Micro:** A specific uniquely shaped tree, a statue in the castle courtyard, a broken cart near a workshop, a particular house with unique (greybox) features.

## Level Map

* A top-down 2D sketch/simple digital drawing showing the overall layout of the castle, village areas, farms, connecting roads, and key building placements.
    
# **Challenges & Rewards**

## Encounters

*(Conceptual, based on placeholder NPC placement and level design)*
*   "Meeting" the Lord of the Castle (approaching the placeholder Lord).
*   "Interacting" with a Villager for a potential task (approaching a placeholder Villager).
*   "Observing" a Blacksmith at work (placeholder dummy at the smithy).
*   "Avoiding" a patrolling Guard (navigating around a placeholder Guard).

## Puzzles

*(Spatial and observational challenges in the greybox)*
*   **Navigation:** Finding optimal or hidden routes through the village and castle.
*   **Stealth Navigation:** Identifying and utilizing cover (bushes, shadows, building corners) to bypass placeholder guards.
*   **Access Puzzles:** Identifying locked doors/chests and the routes to reach them unnoticed.
*   **Environmental Logic:** Understanding how the day/night cycle (conceptual) would affect NPC presence and access to areas.

## Combat

*(Combat is not a primary focus of the greybox implementation, but spaces are designed to support potential future combat)*
*   **Stealth Takedown Spaces:** Areas designed to allow sneaking up behind (placeholder) guards (e.g., blind corners, shadowed alcoves).
*   **Defensive Positions:** Castle walls and towers designed for ranged (placeholder) NPC placement.
*   **Open Areas for Melee:** Village squares or castle courtyards could accommodate future melee encounters.

## Rewards

*(Conceptual rewards the level design provides space/opportunity for)*
*   **Loot Locations:** Placement of chests in villager homes, castle treasury, or hidden areas.
*   **Quest Completion Points:** Designated areas where a player would return to a (placeholder) NPC to "complete" a task.
*   **Exploration Discovery:** Hidden pathways, viewpoints, or small secluded areas that feel rewarding to find.
*   **Safe Zones:** Areas like the Tavern or certain homes that could serve as safe spots or offer respite.

