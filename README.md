# Solutions Team Hiring Assignment

This is the hiring assignment for the Solutions Team at Algolia. It&rsquo;s intended to mimic work you might do here, while giving us an understanding of your skills in:

- Coding
- User Experience
- Communication

If you want to know how we will judge the assignment, you can [view our scoring rubric](scoring-rubric.md).

## Communication Project Instructions

- View the [example customer questions](customer-questions.md)
- Answer them using the Algolia documentation and provide us your answers as a `.txt` file when you email us the rest of your assignment. Please also include them in the same repository as the rest of the assignment.

## Tech and UX Project Instructions

Our sales team has recently been contacted by a large restaurant reservation website, for whom they have identified it to be strategic to build a demo. As a Solutions Engineer, you&rsquo;re asked to build a small prototype that&mdash;using the dataset and UI have provided us&mdash;highlights the benefits of a great search experience.

**Important**: Do not fork this repository to create your assignment. Doing so will wake a bot that prints out your code, immediately sends it to the shredder, and archives your application in our applicant tracking system. And anyway we&rsquo;d rather give everyone an equal shot to show us what they can do.

- Download [the project files](/project-files.zip)
- Push the provided dataset to an Algolia index
- Produce the HTML markup and CSS needed to reproduce the UI provided by the client. To do so, you can write vanilla CSS or with a processor of your choice.
- Using the [Algolia JS Helper](https://community.algolia.com/algoliasearch-helper-js/) and without using instantsearch.js, implement an as-you-type search experience that enables users to easily find restaurants: both by passing a search query and/or filtering on the &ldquo;type of cuisine&rdquo;
- Leverage the user&rsquo;s location to show restaurants closer to them higher in the results&mdash;with a fallback if they dont&rsquo;t allow for geolocation permissions in the browser

![Screenshot](full-version.png)

*Screenshot of a target UI*

#### Important Notes

- Graphical resources, including the Sketch mock-up, are provided in the `./resources` folder
- The mock-up is meant to serve as guidance -- if you have a UI/UX that you believe improves upon the mock-up feel free to implement it, and be ready to explain your choice to do so
- The dataset given by the client is available in the `./resources/dataset folder`. They have been able to extract 5000 restaurants from their database: `restaurants_list.json`. Unfortunately, because of some system complexity on their side, they haven&rsquo;t been able to provide everything in one file only. They have sent us another file named `restaurants_info.csv` that contains additional information for all the extracted restaurants.
  - You&rsquo;ll need to manipulate both data files in order to have access to the &ldquo;type of cuisine.&rdquo;
  - Please include your data manipulation and import script in your Git repository
- **Feel free to use any front-end tooling with which you&rsquo;re most comfortable**
- The blue highlight in the sidebar is an active/hover state
- For payment options, we should **only** have: AMEX/American Express, Visa, Discover, and MasterCard
  - For our purpose, Diners Club and Carte Blanche are Discover cards
- When you sign up for an Algolia account, please put `Interview Candidate` in the company field
  - This helps our sales team know someone's already speaking with you

#### Deliverable

Once you're happy with what you've done

- Publish it using GitHub's gh-pages so we can interact with it
- Send us a link to your finished project via email
- Assignments that do not follow at least the instructions above are not likely to be reviewed highly&mdash;so wow us!

Happy coding!

Note: The provided dataset has been created using the https://github.com/sosedoff/opentable project.
