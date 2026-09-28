# Solutions Engineer Hiring Assignment

This is the hiring assignment for the Solutions Engineering team at Algolia.

The goal of this exercise is to evaluate your ability to understand technical concepts, work with imperfect customer data, build a compelling search experience, and clearly explain the decisions behind your implementation.

## Overview

At a high level, we are asking you to:

1. **Build a working search experience** using the provided OpenTable-style restaurant dataset and a free Algolia trial. You may use InstantSearch.js or another frontend approach of your choice, and any language or tooling you prefer for data preparation and indexing.

2. **Own and explain your technical decisions.** In the technical debrief, be prepared to explain what you built, what you changed, challenges you encountered, and why you made specific architecture, data, and search configuration decisions. You are responsible for understanding every configuration or setting applied to your implementation, whether you selected it yourself, found it in documentation, or used AI to recommend or generate it. Understanding the configuration is equally as important as the output.

3. **Go beyond making search technically work.** Explore the dataset, test realistic searches and refinements, identify where results are and are not relevant, and iteratively tune the experience. We want to see how you reason about search quality, not just whether you can create an index and search it.

4. **Use the tools available to you.** Algolia documentation, Algolia AI Assist, coding assistants, and other AI tools are all encouraged for learning, coding, debugging, data manipulation, and exploring configuration options. AI can help you move faster, but you should be able to explain what was implemented, why it is appropriate for this use case, and how it affects the search experience.

5. **Approach the exercise as a Solutions Engineer.** Build and present the experience as if you were preparing for a customer meeting. Connect your implementation, relevance tuning, and product decisions to the customer problems and opportunities described in the assignment, and be prepared to communicate your choices to both technical and non-technical stakeholders.
## Prospect Context: Account Executive Discovery Notes

Please refer to prospect-context.md

## Technical and UX Project Instructions

Our sales team has recently been contacted by OpenTable.

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

Feel free to enrich the data with any additional information you think would be useful for discovery purposes.

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

From the Algolia dashboard, provide personification access for our team:

- Navigate to Settings → Support Access
- Enable "Allow Algolia employees to access my account"

When you are ready to submit, please send us:

- A link to the live demo, for example via GitHub Pages, Vercel, Netlify, or another hosting option
- A link to your Git repository
- A short explanation of your approach

## What Happens Next

Please refer to interview-next-steps.md
