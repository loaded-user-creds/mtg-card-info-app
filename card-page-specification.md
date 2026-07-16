# Mobile Card Page Specification

The card page is the center of the application. It should feel familiar to anyone who has used an MTG card database, but it must make the difference between the card and a specific printing clear at all times.

## Page structure

The approved mobile layout is:

1. Card image and printing selector
2. Universal card information
3. Selected-printing information
4. Discussion
   - All Printings
   - This Printing

The page is designed for a phone first. Important information should be visible without turning the screen sideways or opening a desktop-style table.

## 1. Card image and printing selector

The top of the page should contain a large card image and enough printing information to identify what is currently being shown.

Recommended visible details:

- Card name
- Set name and set symbol
- Collector number
- Release year
- Rarity
- Finish or treatment when relevant

The user should be able to swipe left or right between printings. Swiping should not be the only control because some cards have many versions.

An **All Printings** button should open a searchable selection panel with image thumbnails. Useful filters may include:

- Set
- Year
- Language
- Foil or nonfoil
- Frame or treatment
- Promotional release

### Default printing behavior

The app should use the following order when deciding which printing to show:

1. The printing the user previously selected
2. The printing opened from search, a notification, or an external link
3. The most recent standard English tabletop printing
4. A designated representative printing

A promotional or unusual treatment should not become the default simply because it is the newest version.

## 2. Universal card information

This section contains information that belongs to the card across printings.

Depending on the card, it may include:

- Mana cost
- Mana value
- Color
- Color identity
- Card type and subtype
- Oracle text
- Power and toughness
- Loyalty
- Defense
- Format legality
- Official rulings
- Keyword definitions

The card image already displays much of this information, so the section should be compact and easy to expand rather than visually repeating the entire card.

The data model and interface must support cards with more than one face or layout, including double-faced, split, adventure, prototype, and other nonstandard cards.

## 3. Selected-printing information

This section changes when the selected printing changes.

It may include:

- Set name and code
- Set symbol
- Collector number
- Release date
- Rarity
- Artist
- Language
- Foil availability
- Current finish
- Frame or special treatment
- Promotional status
- Available market information and its last-updated date

This information should remain separate from the universal card information. That separation is important to both the interface and the underlying data model.

## 4. Discussion

The discussion area should use a sticky segmented control rather than placing two long feeds one after the other.

```text
[ All Printings ]  [ This Printing ]
```

The selected printing should be identified clearly above the printing-specific feed and while a post is being written.

Example:

```text
THIS PRINTING
Modern Horizons 3 · #162 · Borderless Foil
```

### All Printings

This feed is for subjects that apply to the card generally:

- Gameplay
- Rules and interactions
- Deckbuilding
- Combos and synergies
- Card history and artwork
- Reprints
- General questions

### This Printing

This feed is for subjects tied to the selected physical release:

- Pricing and collecting
- Condition and grading
- Identification and counterfeits
- Print quality and defects
- Foiling and curling
- Availability and distribution
- Other printing-specific discussion

### Categories and filters

Categories should be attached to posts and used as feed filters. They should not become separate subforums in the first version.

This keeps related discussion together, reduces empty sections, and makes it easier to browse on a phone.

## Post scope

Every post should visibly show its scope.

Examples:

```text
ALL PRINTINGS
Rules & Gameplay
```

```text
SPECIFIC PRINTING
Alpha · #161 · Nonfoil
Condition & Grading
```

The posting interface should require the user to confirm whether the post applies to all printings or only the selected printing. This is one of the most important protections against misplaced information.

## Basic mobile behavior

The first prototype should account for:

- A persistent back button or navigation control
- Saving or following a card
- Sharing the current card or printing
- Loading and empty states
- Cards with a very large number of printings
- Cards without market information
- Cards with multiple faces
- Long Oracle text
- Discussion feeds with no posts
- Clear reporting controls on community content

## Open design questions

These details have not been finalized:

- Whether pricing appears directly in the printing section or behind a secondary view
- Whether official rulings are expanded inline or opened separately
- How many printing thumbnails appear before search or filters are needed
- Whether comments use a fully threaded structure or a simpler reply model
- How voting, accepted answers, or usefulness markers should work
- Which actions remain available to users who are not signed in
