# Phase 2: Flux Architecture and Projects CRUD (2.5 days)

## Rails
### Models
* Project

### Controllers
Api::ProjectsController

### Views

## Flux
### Views (React Components)
ProjectsIndex.jsx
Project.jsx
Form.jsx

### Stores
Project.js

### Actions
ApiAction.receiveAllProjects -> triggered by ApiUtil
ApiActions.receiveProject
ApiAction.deleteProject
ProjectActions.fetchAllProject -> triggers ApiUtil
ProjectActions.createProject
ProjectActions.editProject
ProjectActions.destroyProject

### ApiUtil
ApiUtil.js

## Gems/Libraries
* JQuery
* Flux
* react-router { Route Router }
* react-dom
* babel-core babel-loader babel-preset-react
