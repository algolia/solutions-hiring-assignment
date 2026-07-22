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

Please refer to prospect-context.md

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

From the Algolia dashboard provide personification access for our team
  - Navigate to Settings → Support Access 
  - Enable "Allow Algolia employees to access my account"

When you are ready to submit, please send us:
- A link to the live demo, for example via GitHub Pages, Vercel, Netlify, or another hosting option
- A link to your Git repository
- A short explanation of your approach

## What Happens Next

Please refer to interview-next-steps.md

