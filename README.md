# MTG Card Info App

A mobile-first reference and discussion app where every Magic: The Gathering card has a useful home of its own.

## The idea

Card-specific knowledge is scattered across Reddit, Discord, YouTube, marketplaces, deck apps, forums, and social media. Useful conversations are hard to find later, and most card apps are built around deck construction, collection tracking, pricing, or buying and selling.

This project takes a different approach: the card page is the center of the experience. A user can search for a card, move between its printings, review information about the card or a particular release, and join a discussion without digging through unrelated threads.

The first version is focused on Magic: The Gathering. It is intended for players, collectors, buyers, sellers, and other experienced users who want more than rules text or a current price.

## How the card page works

The approved mobile card page has four parts:

1. **Card image and printing selector** — The page opens on the user's last-selected printing or the printing that brought them to the page. Otherwise, it uses the most recent standard English tabletop printing or a designated representative printing. Users can swipe between printings or open a searchable **All Printings** selector.
2. **Universal card information** — Details shared by every printing, including the card's name, rules text, mana cost, type line, and other gameplay information.
3. **Selected-printing information** — Details tied to the printing currently on screen: set, release date, collector number, rarity, artist, finish, treatment, language, market price, and the time of the latest price update.
4. **Discussion** — Two tabs keep general and printing-specific conversations together without mixing them up:
   - **All Printings** covers gameplay, rules, deckbuilding, card history, artwork, and other topics that apply to the card as a whole.
   - **This Printing** covers price, condition, grading, identification, counterfeit concerns, print quality, and other details unique to a particular release.

Printing-specific topics will use categories and filters inside **This Printing**, not a collection of separate subforums.

## First-release scope

The planned MVP includes:

- User accounts
- A searchable MTG card database
- A dedicated page for each card and its printings
- Posts and replies
- Voting to help useful contributions rise to the top
- Topic labels and discussion filters
- Reporting and basic moderation tools
- Saved cards and followed discussions
- Notifications

## What it is not

The first release is not intended to be a marketplace, deck builder, or full collection tracker. It will not include direct sales or payment processing, private trading, automated grading, AI-generated valuations, live auction data, or video feeds. Support for other trading card games may be considered later, but it is outside the initial scope.

## Product documentation

- [Product brief](product-brief.md)
- [Mobile card page specification](card-page-specification.md)
- [Product decisions](product-decisions.md)
- [Development roadmap](development-roadmap.md)

## Project status

The initial product-definition stage is complete. The product brief, core product decisions, and canonical mobile card-page structure are approved. The project is ready to begin low-fidelity prototyping. No application stack has been selected and no production code has been written.

The next step is a low-fidelity clickable prototype. That prototype will be tested with Magic players and collectors before technical design and development begin.

## Current roadmap

1. Organize the product definition — **Complete**
2. Create low-fidelity mobile wireframes — **Next**
3. Test the concept with players and collectors
4. Complete technical discovery
5. Build the MVP
6. Conduct private testing
7. Begin a limited public release

---

Magic: The Gathering is a trademark of Wizards of the Coast. This is an independent project and is not affiliated with or endorsed by Wizards of the Coast.
