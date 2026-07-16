# Product Decisions

This file records decisions that have already been made so they do not have to be reconsidered every time the project moves into a new phase.

## 1. Start with Magic: The Gathering

**Decision:** The first version will focus on Magic only.

**Reason:** Supporting every trading card game would multiply the data, terminology, licensing, moderation, and interface problems before the basic idea has been tested.

Expansion can be considered later if the structure works well for Magic users.

## 2. Build a focused companion app

**Decision:** The initial product will not try to replace ManaBox, TCGplayer, Gatherer, Reddit, or Discord in every area.

**Reason:** Those products already have strong positions in deck building, collection management, buying and selling, official reference material, and general community discussion.

The app should be best at persistent, searchable, card-specific knowledge and conversation.

## 3. Treat the card and its printings as separate objects

**Decision:** General card information and discussion will be separated from printing-specific information and discussion.

**Reason:** Rules, gameplay, and deckbuilding usually apply to the card as a whole. Price, condition, print defects, grading, and counterfeit concerns often apply to one release.

This distinction is the core of the product.

## 4. Use one card page with a printing selector

**Decision:** A card page will show one selected printing at a time, with swipe controls and an All Printings selector.

**Reason:** This keeps the mobile page understandable while still giving access to every release.

## 5. Use a predictable default printing

**Decision:** The app will prefer the user's last selection or the printing that led them to the page. Otherwise, it will normally show the most recent standard English tabletop printing or a chosen representative printing.

**Reason:** “Most popular” is difficult to define consistently. A predictable rule is easier for users to understand and easier to implement.

## 6. Use tabs for discussion scope

**Decision:** Discussion will use **All Printings** and **This Printing** tabs.

**Reason:** Stacking two discussion feeds vertically would be confusing on a phone and would make it easier to post in the wrong place.

## 7. Use categories, not separate subforums

**Decision:** Pricing, grading, identification, gameplay, and similar topics will be post categories and filters.

**Reason:** Creating a separate forum for each category would produce many empty sections, especially on less popular cards.

## 8. Design for mobile first

**Decision:** The first wireframes and product behavior will be designed for a phone.

**Reason:** Card lookup often happens at a game store, event, trade table, or while viewing a physical collection. The phone experience is the primary use case.

A desktop or tablet layout can be adapted later.

## 9. Do not build a marketplace in the first version

**Decision:** Buying, selling, payment processing, and private trades are outside the MVP.

**Reason:** A marketplace introduces payments, fraud, disputes, shipping, seller reputation, legal requirements, and direct competition with established platforms. It would distract from testing the core knowledge and discussion concept.

## 10. Do not choose the technology stack yet

**Decision:** The project will complete a clickable prototype and basic user testing before committing to a programming language, framework, database, or hosting provider.

**Reason:** The interface and user behavior should be tested before technical choices make the product expensive to change.
