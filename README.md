# PlazaRouting OpenAPI Specification
[![Build Status](https://travis-ci.org/PlazaRoute/api.svg?branch=master)](https://travis-ci.org/PlazaRoute/api)

## Links

- Documentation(ReDoc): https://plazaroute.github.io/api/
- SwaggerUI: https://plazaroute.github.io/api/swagger-ui/
- Look full spec:
    + JSON https://plazaroute.github.io/api/swagger.json
    + YAML https://plazaroute.github.io/api/swagger.yaml
- Preview spec version for branch `[branch]`: https://plazaroute.github.io/api/preview/[branch]

**Warning:** All above links are updated only after Travis CI finishes deployment

## Working on specification
### Install

1. Install [Node JS](https://nodejs.org/)
2. `npm install -g yo`
3. `npm install -g generator-openapi-repo`
4. clone repo
5. `yo openapi-repo`

### Usage

1. start local flask server and go to http://localhost:5000/api/swagger.json
2. save swagger.json to `spec/`
3. replace `"host": "localhost:5000"` with
```,
"host": "plazaroute.infs.ch",
"schemes": ["https"]
```
4. delete `spec/swagger.yaml`
5. `yo openapi-repo` and make sure not to override the README
6. push changes
