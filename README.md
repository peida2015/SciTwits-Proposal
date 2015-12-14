# SciTwits

## Minimum Viable Product

SciTwits is a web application inspired by StockTwits and to be built with Ruby on Rails and React.js.  SciTwits allow users to:

- [ ] Create an account
- [ ] Log in / Log Out
- [ ] Create research project (Become owner)
- [ ] Provide (multimedia) description of project (called 'Showcase')
- [ ] Add members to project if user is owner
- [ ] Submit Twits about a project
- [ ] View number of followers
- [ ] Follow projects
- [ ] For all users (without logging in), see a heatmap of research similar to StockTwits's

NB: Heatmap will be generated using data from PLoS Article Level Metric (ALM) API and graphing capabilities of Highcharts JS charting library.

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
views for the Project `Index`, `IndexItems` and `Form`. At the end of Phase 2,
Projects can be created, read, edited and destroyed in the browser.
Projects should save to the database when the form loses focus or is left idle
after editing.

### Phase III: 
