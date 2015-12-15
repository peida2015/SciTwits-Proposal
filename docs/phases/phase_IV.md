# Phase 4: Follows Flux and CRUD (1 day)

## Rails
### Models
* Follows

### Controllers
Api::FollowsController (create, destroy)

### Views
follows/index.json.jbuilder

## Flux
Follows
### Views (React Components)
Project.jsx
FollowsButton.jsx (nested under Project)
FollowsStat.jsx

### Stores
FollowsStore.js

### Actions
FollowAction.createFollow -> triggers ApiUtil
FollowAction.destroyFollow
FollowAction.receiveAllFollows(project)

### ApiUtil
ApiUtil.js

## Gems/Libraries
* JQuery
* Flux
* react-router { Route Router }
* react-dom
* babel-core babel-loader babel-preset-react
