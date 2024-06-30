# CasaVue demo
https://demo.casavue.app

## Repo content
This repo is a simple example of how [CasaVue](https://casavue.app) can be used to generate a static home page.

Page deployment consists of two steps:
- [`build-config`](https://github.com/czoczo/casavue-demo/blob/main/.github/workflows/build-demo-page.yaml#L15) - using [`items_config_generator.py`](https://github.com/czoczo/casavue-demo/blob/main/items_config_generator.py) script to generate CasaVue [`items.yaml`](https://casavue.app/configuration/file/#static-items-definitions) configuration file based on [Awesome-Selfhosted Github repo](https://github.com/awesome-selfhosted/awesome-selfhosted). 
- [`build-casavue-static-content`](https://github.com/czoczo/cavude/blob/main/.github/workflows/build-demo-page.yaml#L37) - using CasaVue [static mode](https://dev.casavue.app/deployment/deploy_docker/#static-mode) to generate content for deployment on Github Pages.

All steps are implemented in [Github Workflow](https://github.com/czoczo/casavue-demo/blob/main/.github/workflows/build-demo-page.yaml).