# Introduction 

Not sure exactly what will go here, but starting with some OpenAPI-linting rules, and starting with specifying them using the Spectral v6 standard.

# Notes

* As of the moment I wrote this, [OpenAPI's example API](https://raw.githubusercontent.com/OAI/OpenAPI-Specification/d5307aff5debf8fc895208235cc90976d67e7f3a/examples/v3.0/api-with-examples.yaml) failed my rulesets, which is awesome, because you can see if the rules catch it.
    1. Shell invocation:
       ```sh
       npx @stoplight/spectral-cli lint https://raw.githubusercontent.com/OAI/OpenAPI-Specification/d5307aff5debf8fc895208235cc90976d67e7f3a/examples/v3.0/api-with-examples.yaml --ruleset https://raw.githubusercontent.com/kkgthb/api-spec-analysis-01-playing/main/resources/rulesets/spectral/.spectral.yaml
       ```
    1. [VSCode extension](https://marketplace.visualstudio.com/items?itemName=stoplight.spectral)
* I have no idea how I want to structure this.  For now, taking a page from [Microsoft](https://github.com/Azure/APICenter-Analyzer/) and putting the Spectral-formatted specs in under `/resources/` folder.
* Learned "extends" format from [SPS](https://github.com/SPSCommerce/sps-api-standards/blob/main/rulesets/src/.spectral.yml) as linked by [Stoplight, Spectral's main maintainer](https://github.com/stoplightio/spectral-rulesets?tab=readme-ov-file#spectral-rulesets).
