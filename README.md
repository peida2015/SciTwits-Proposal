# SciTwits

[SciTwits][SciTwits]
[SciTwits]:http://scitwits.heroku.com

## Minimum Viable Product

SciTwits is a web application inspired by StockTwits and Kickstarter, and will
be built with Ruby on Rails and React.js.  SciTwits allow users to:

- [ ] Create an account
- [ ] Log in / Log Out
- [ ] Create research project (Become owner)
- [ ] Provide (multimedia) description of project (called 'Showcase')
- [ ] Submit Twits about a project
- [ ] View number of followers
- [ ] Follow projects

NB: Heatmap will be generated using data from user Followings or PLoS Article Level Metric (ALM) API and graphing capabilities of Highcharts JS charting library.

## Design Docs

* [View Wireframes][view]
* [DB schema][schema]

[view]: ./docs/views.md
[schema]: ./docs/schema.md

## Implementation Timeline

### Phase I: User Authentication, Project Model and JSON API (1.5 days)

In Phase 1, I will begin by implementing user signup and authentication (using
BCrypt). There will be a basic landing page after signup that will contain the
container for the application's root React component. Before building out the
front end, I will begin by setting up a full JSON API for Projects.

### Phase II: Flux Architecture and Projects CRUD (2.5 days)
Phase 2 is focused on setting up Flux, the React Router, and the React view
structure for the main application. After the basic Flux architecture has been
set up, a Note store will be implemented and a set of actions corresponding to
the needed CRUD functionality created. Once this is done, I will create React
views for the `ProjectsIndex`, `Project` and `Form`. At the end of Phase 2,
Projects can be created, read, edited and destroyed in the browser.
Projects should save to the database when the form loses focus or is left idle
after editing.

### Phase III: Twits Flux and CRUD(1 day)
I will add the ability to add and reply to twits about a project for users.  
'Twits' and 'Twit' components will be added to React views for 'Project'.  Twits can be saved to or deleted from database.  'Tags' will be added on each twit.

### Phase IV: Heatmap and Following Stats (2 days)
For each project, user can follow or unfollow a project.  A 'heatmap' component
added to the 'ProjectsIndex' will be generated based on the number of followings for each project.  Highcharts JS library will be used.  A stats section will be added to the header.

### Phase V: Styling with CSS and database seeding (2 days)
In this final phase, I will add styling to the pages and seed the database with ipsum.


## Bonus
- [ ] users can support a project
- [ ] owner can add another member to a project
- [ ] a heatmap of research projects similar to StockTwits's
