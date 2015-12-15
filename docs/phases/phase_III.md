# Phase 3: Twits Flux and CRUD(1 day)

## Rails
### Models
* Twit

### Controllers
Api::TwitsController (create, destroy, index)

### Views
twits/index.json.jbuilder

## Flux
Twits
### Views (React Components)
Project.jsx
Twits.jsx (nested under Project)
TwitsForm.jsx

### Stores
TwitStore.js

### Actions
TwitAction.createTwit -> triggers ApiUtil
TwitAction.destroyTwit
TwitAction.receiveAllTwits(project)

### ApiUtil
ApiUtil.js

## Gems/Libraries
* JQuery
* Flux
* react-router { Route Router }
* react-dom
* babel-core babel-loader babel-preset-react
