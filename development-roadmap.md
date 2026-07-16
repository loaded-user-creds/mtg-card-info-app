# Development Roadmap

This roadmap is intentionally practical. The project should earn its way from one stage to the next rather than jumping directly into a large application build.

## Stage 1: Organize the product definition

**Status:** Complete

Goals:

- Keep the product brief current
- Record decisions as they are made
- Define the mobile card-page structure
- Identify assumptions that still need testing
- Keep the repository understandable to someone joining the project later

Exit point:

- The product purpose, initial audience, MVP, and non-goals are clear

## Stage 2: Create low-fidelity wireframes

**Status:** Next

Goals:

- Design the home and search screens
- Design search results
- Design the approved card page
- Design the printing selector
- Design both discussion views
- Design a discussion thread
- Design the create-post flow
- Include empty, loading, and error states

The wireframes do not need polished artwork or branding. They need to show how a user moves through the product and where each piece of information belongs.

Exit point:

- A clickable mobile prototype can complete the main lookup and discussion flows

## Stage 3: Test the idea with users

Goals:

- Show the prototype to Magic players and collectors
- Ask users to find a card and a specific printing
- Test whether they understand All Printings versus This Printing
- Observe where they hesitate instead of explaining the interface first
- Ask what information they expected but could not find
- Determine whether they would install and revisit the app

A small number of thoughtful interviews is more useful at this point than a large general survey.

Exit point:

- The core page structure is understood without coaching
- At least one repeat-use case is supported by user feedback
- Major usability problems have been corrected

## Stage 4: Technical discovery

Goals:

- Evaluate card-data sources and usage requirements
- Determine how card identities and printings will be stored
- Decide how card images will be referenced and cached
- Choose authentication and account requirements
- Define posts, comments, votes, reports, follows, and notifications
- Estimate moderation needs
- Select the application framework, backend, database, and hosting approach
- Build one small technical test before committing to the full stack

Important questions:

- How will card data stay current?
- Which data can be stored locally and which must be requested?
- How will reprints and unusual card layouts be represented?
- How will public discussion pages be indexed and shared?
- What information requires attribution or specific licensing treatment?

Exit point:

- A written technical plan and a working data/search experiment exist

## Stage 5: Build the MVP

Suggested build order:

1. Card-data import or API connection
2. Search
3. Card and printing views
4. User accounts
5. Posts and replies
6. Discussion scope and categories
7. Following and notifications
8. Reporting and moderation
9. Basic analytics and error tracking

The first build should prioritize a complete narrow path over a large number of unfinished features.

Exit point:

- A user can search for a card, select a printing, read both discussion scopes, create a post, and receive a reply

## Stage 6: Private testing

Goals:

- Invite a small group of players and collectors
- Seed useful discussions on selected cards
- Watch for empty-page behavior
- Test moderation and reporting
- Measure return visits and contribution rates
- Fix reliability and navigation problems

Exit point:

- The app is stable enough for a wider audience
- The team understands which cards and topics create repeat activity

## Stage 7: Limited public release

Goals:

- Launch with a focused set of promoted cards, sets, or topics
- Publish clear community guidelines
- Respond quickly to reports and data problems
- Track search success, follows, posts, replies, and return use
- Avoid adding large adjacent features until the core behavior is proven

## Items to defer

Unless user testing changes the product direction, these should remain outside the early roadmap:

- Marketplace and payments
- Private card trading
- Full collection tracking
- Deck construction
- Automated card grading
- Support for other card games
- Advanced price forecasting
- General-purpose social feeds

## Next action

Create the first low-fidelity mobile wireframe for the card page, using the approved structure in [card-page-specification.md](card-page-specification.md).
