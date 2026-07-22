# Solutions Engineer Hiring Assignment

This is the hiring assignment for the Solutions Engineering team at Algolia.

The goal of this exercise is  to test your ability to understand technical concepts, explain them clearly, manipulate data and build demos (with your preferred tooling). We expect strong SEs to use the tools available to them to move faster, explore ideas, and deliver better outcomes for prospects.

What we care about is your ability to:

- Understand Algolia's core technical concepts
- Transform messy customer data into a useful search index
- Design a relevant and compelling search and discovery experience
- Make thoughtful architecture and implementation decisions
- Evaluate search quality and tune configuration accordingly
- Communicate your choices clearly to both technical and non-technical audiences

You are welcome, and encouraged, to use AI tools to help you write code, manipulate data, generate UI ideas, debug, or accelerate implementation. Be ready to explain the concepts, architecture, trade-offs, and decisions behind what you built.

## Prospect Context: Account Executive Discovery Notes

Before starting the assignment, assume you have received the following discovery notes from the Account Executive working on the opportunity.

The prospect is **OpenTable**, a large restaurant reservation platform. They currently rely on an in-house search and discovery experience built on top of Elasticsearch. This search stack was originally developed around 10 years ago and is now considered old, difficult to evolve, and no longer aligned with the experience they want to offer users.

OpenTable is looking for a more modern and higher-quality search and discovery experience. Their goal is to increase usage of the platform and improve conversion from search or discovery sessions into restaurant bookings.

### User Personas

OpenTable has two main types of users.

#### 1. Users who know exactly what they are looking for

These users come to OpenTable knowing what they are looking for. They often know the restaurant name and want to find the right restaurant quickly so they can book a table.

Current pain points include:

- Restaurant names can be hard to spell or remember
- Typos, concatenated words, partial names, or alternate spellings can lead to poor results
- Some restaurant chains have multiple locations in the same city, making it hard for users to identify the correct one

For this persona, the experience should make known-item search fast, forgiving, and precise.

#### 2. Users who do not know what they are looking for yet

These users come to OpenTable to explore. They may not have a specific restaurant in mind and instead want to browse, compare options, and get inspired.

Current pain points include:

- The current experience does not support discovery well
- Users have limited ways to browse, refine, or get inspired
- The experience feels less modern than what users expect from consumer discovery platforms

For this persona, the experience should help users discover restaurants using useful browsing, filtering, sorting, and search experiences.

### Business Goals

OpenTable wants to improve the experience for both users who know what they are looking for and users who are exploring options.

The desired outcomes are:

- Higher search quality
- A more modern user experience
- Better support for restaurant discovery and inspiration
- Increased platform usage
- Increased conversion from search or browsing sessions into bookings

As you design your solution, use this discovery context to guide your decisions. Your demo should not only show that Algolia can return results; it should show how Algolia could help OpenTable create a better end-user experience and achieve these business goals.

## Communication Project Instructions

View the [example customer questions](customer-questions.md) and answer them using the Algolia documentation.

Please include your answers in your repository. A `.txt`, `.md`, or similar plain-text format is fine.

We are evaluating how clearly you can explain technical topics to a customer. Strong answers should be accurate, concise, and adapted to the customer's likely level of understanding.

## Technical and UX Project Instructions

Our sales team has recently been contacted by OpenTable.&#x20;

As a Solutions Engineer, your task is to build a small interactive prototype using the provided restaurant dataset. Your demo should highlight the value of a great search and discovery experience, using the discovery notes above as your guide.

This is not a pixel-perfect implementation exercise. The provided mock-up represents OpenTable's current experience. It is included to give you context on what they have today, but the prospect does not want to simply recreate this experience. They are looking for something better: a more modern, more useful, and more compelling search and discovery experience.

We encourage you to innovate. Show us how you would bring a prospect a vision, not just a functional search box.

**Important:** Do not fork this repository to create your assignment. Create your own private or public repository for your work and send us the link when you submit.

## What You Should Build

Download [the project files](/project-files.zip), then build a working restaurant discovery demo.

Your demo should include the following:

- An Algolia index populated with the provided restaurant data
- A data preparation process that combines and cleans the provided files
- A search interface that lets users find restaurants through text search
- Relevant filtering or refinement, including cuisine type
- Location-aware ranking, or a thoughtful fallback if browser geolocation is not available
- Search configuration that you have tested and tuned based on the dataset
- A user experience that demonstrates how OpenTable's search and discovery experience could be improved for both known-item search and open-ended discovery

You may use any front-end framework, tooling, UI library, or AI coding assistant you prefer. However, for the core search implementation, please use the [Algolia JS Helper](https://community.algolia.com/algoliasearch-helper-js/) and do not use InstantSearch.js.

This constraint is intentional: we want to understand how you think about search state, queries, refinements, results, and UI behavior rather than only how you assemble pre-built widgets.

Choose the implementation approach that lets you best demonstrate your understanding of Algolia and your ability to deliver value quickly.

## Data Requirements

The dataset is available in the `./resources/dataset` folder.

The client has provided two files:

- `restaurants_list.json`, containing approximately 5,000 restaurants
- `restaurants_info.csv`, containing additional information about those restaurants

Because the data is split across files, you will need to manipulate and combine them before indexing.

Your indexed records should include the information needed to support the search experience, including cuisine type.

Please include your data manipulation and import script in your repository. AI assistance is allowed, but you should be able to explain:

- How the files were joined
- What transformations or cleanup you performed
- Which attributes you indexed
- Which attributes you made searchable, facetable, or ranking-related
- Any assumptions you made about the data

Feel free to enrich the data with any additional information you think would be useful for discovery purposes

## Search and Relevance Requirements

Do not stop once search technically works. Test it as if you were preparing for a customer meeting.

Try representative searches and refinements, inspect the results, and adjust the index configuration where needed.

We are interested in how you think about relevance. Your submission should show evidence that you considered topics such as:

- Searchable attributes
- Ranking and custom ranking
- Facets and filters
- Geo-search or location-based relevance
- Typo tolerance and query behavior
- Result ordering and perceived quality
- How the experience should behave when the query is broad, specific, misspelled, ambiguous, location-sensitive, or empty

You do not need to find a perfect configuration. We want to see that you can reason about search quality, test your assumptions, and improve the experience iteratively.


## Deliverables

When you are ready to submit, please send us:

- A link to the live demo, for example via GitHub Pages, Vercel, Netlify, or another hosting option
- A link to your Git repository
- Your answers to the communication project questions
- A short explanation of your approach

## What Happens Next

If you pass the technical assignment step, there will be two follow-up interview calls.

### 1. Technical Debrief

The first call will be a technical debrief.

You will have 20-25 minutes to explain what you built, including:

- The technical choices you made
- Why you built the solution the way you did
- How you structured the data and indexed it in Algolia
- How you configured Algolia and tuned relevance
- Any problems, trade-offs, or challenges you encountered while building the demo
- What you would improve with more time

We will then ask questions to better understand your implementation and challenge some of your choices. You should also be prepared to show the front-end experience and the Algolia configuration, and explain why your choices make sense for a prospect like OpenTable.

### 2. Mock Customer Call

The second call will be a 45-minute mock customer call.

In this scenario, two Algolia interviewers will play the roles of OpenTable stakeholders: typically a CTO and a CPO.

You should prepare to present your demo as if you were the Solutions Engineer on the opportunity. You will have around 20-25 minutes to:

- Set the context for the conversation
- Ask any additional discovery questions you think are important
- Present the demo you built
- Explain how your solution addresses OpenTable's user pains and business goals
- Highlight the Algolia capabilities and configuration choices that matter most for this prospect

The remaining 10-15 minutes will be used for questions and discussion.

The goal of this call is not only to evaluate the demo itself, but also how you run a customer-facing technical conversation: how you connect the solution to the prospect's needs, how you explain technical concepts, and how you handle questions from business and technical stakeholders.

Have fun with the assignment. We are excited to see how you would imagine a better restaurant discovery experience.
