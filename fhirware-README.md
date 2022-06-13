## FYI: the fhirware project vs this copy of it

This readme file is the readme file for [the fhirware project](https://github.com/ShahimEssaid/fhirware). Please see [the upstream version]() of this readme if you would like to learn about the fhirware project itself. The rest of this readme is likely an older copy of the upstream version, and that's only applicable to this copy of the upstream repository.

If you are reading this at its upstream repository, i.e. [here](https://github.com/ShahimEssaid/fhirware), do not clone this repository before you read the rest of this readme and understand the few options you have for reusing this content.

The documentation is minimal and possibly not fully accurate at this point but will improve soon.

## The fhirware project

This repository aims to provide various FHIR-related content and configurations that might help you with your FHIR related project(s). This project is still a work in progress, somewhat unstable, but still useful enough to give it a try if you like.

It provides:
* A GitHub Actions based IG automated build and publication, per branch and per PR. It uses a Docker image from [this repository](https://github.com/ShahimEssaid/docker-hl7-fhir-ig-publisher) published [at dockerhub](https://hub.docker.com/r/sessaid/ig-publisher)
* VS Code configuration to enable JSON Schema and Yaml auto complete and validation for FHIR resource files under the `fw-examples` directory.
* Two template IGs to get started.


## Getting started

This repository is intentionally set as a template repository to prevent forks. The idea is that you have your own repository, or create one, and then get this content into your repository. You can do both of those steps by clicking on the ` use this template` button but that will create a repository that is disconnected from this repository and make future updates more difficult. Another option, if you're starting from scratch, is to do a local clone and push it to your own GitHub repository. If you already have a repository, you can use git merge like this: `git merge --allow-unrelated-histories fhirware/main` after you add this repository as a remote. All content at the root is intentionally `fw-` prefixed to minimize name collision with your content. The other option is to use `git subtree`.

This repository is used with `git merge....` at my [fhir-demo](https://github.com/ShahimEssaid/fhir-demo) repository for testing and demonstration purposes. You might need to look at the dev branch until it's merged into main.

The other readmes in the subfolders are still work in progress and might be misleading. Please reach out by opening an issue if needed until I have the time for better documentation.