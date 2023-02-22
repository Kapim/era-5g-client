# era-5g-client
Python client for Net Applications.

## Contributing, development

- Any contribution should go through a pull request from your fork.
- Before commiting, please run locally:
  - `./pants fmt ::` - format all code according to our standard.
  - `./pants lint ::` - checks formatting and few more things.
  - `./pants check ::` - runs type checking (mypy).
- The same checks will be run within CI.
- A virtual environment with all necessary dependencies can be generated using `./pants export ::`.
- To generate distribution packages (`tar.gz` and `whl`), you may run `./pants package ::`.
- For commit messages, please stick to [https://www.conventionalcommits.org/en/v1.0.0/](https://www.conventionalcommits.org/en/v1.0.0/).
- The package depends on `opencv-contrib-python`, but for full functionality, one has to compile OpenCV with support for GStreamer (we will provide pre-compiled whl in a near future).