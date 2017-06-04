# Thing FSM (Field Service Management) OpenAPI Specification
[![Build Status](https://travis-ci.org/ZoetropeLabs/thing-fsm.svg?branch=master)](https://travis-ci.org/ZoetropeLabs/thing-fsm)

this is an API specification to allow IoT platforms to push IoT device service alerts and faults to FSM (Field service management) software. It's been created as an open standard to allow interoperable IoT and FSM systems where each system will only need to implement once in order to gain broad compatibility.
    
This documents a set of endpoints which should be exposed by the service management software, however does not dictate how the events should be processed by the FSM software, though in most cases it's expected that `warning` or greater level events will be raised as service jobs automatically.

FSM and IoT service providers are encouraged to help shape the development of this standard by raising pull requests and getting involved with suggestions. We're currently working towards a 1.0.0 release, however implementations of this standard are already underway.

IoT platforms can implement web-hooks which corrispond to this API in order to transfer events to FSM software in a standardised way.

Created by [ZConnect](https://zconnect.io) for the good of the industry.

## Links

- Documentation(ReDoc): https://zoetropelabs.github.io/thing-fsm/
- SwaggerUI: https://zoetropelabs.github.io/thing-fsm/swagger-ui/
- Look full spec:
    + JSON https://zoetropelabs.github.io/thing-fsm/swagger.json
    + YAML https://zoetropelabs.github.io/thing-fsm/swagger.yaml
- Preview spec version for branch `[branch]`: https://zoetropelabs.github.io/thing-fsm/preview/[branch]

**Warning:** All above links are updated only after Travis CI finishes deployment

## Working on specification
### Install

1. Install [Node JS](https://nodejs.org/)
2. Clone repo and `cd`
    + Run `npm install`

### Usage

1. Run `npm start`
2. Checkout console output to see where local server is started. You can use all [links](#links) (except `preview`) by replacing https://zoetropelabs.github.io/thing-fsm/ with url from the message: `Server started <url>`
3. Make changes using your favorite editor or `swagger-editor` (look for URL in console output)
4. All changes are immediately propagated to your local server, moreover all documentation pages will be automagically refreshed in a browser after each change
**TIP:** you can open `swagger-editor`, documentation and `swagger-ui` in parallel
5. Once you finish with the changes you can run tests using: `npm test`
6. Share you changes with the rest of the world by pushing to GitHub :smile:

API to allow IoT platforms to push IoT device service alerts and faults to FSM software. Created as an open standard for the good of the industry