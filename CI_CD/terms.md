https://rollout.io/blog/beginners-guide-to-continuous-integration-and-deployment/

* **Environment** - system used in the project, ex. Develop, Test, Production
* **Build** - version of the software; setting up a version of the software
* **Phase** - stages of building environment, ex. clone> build> unit tests> deploy
* **Job** - a task carried out during a phase of environment setup, ex. install dependencies, import database, add environment variables, run tests
* **Pipeline** - linear progress of development/deployment process ex. merge > build > unit test > deploy on dev > UI test > build on prod
#### Container
- an abstraction layer that virtualizes the operating system; a package of software, all of its dependencies and OS spec; kinda similar to CD image
#### Virtual environments - venv
- enables creating an environment according to specification (what software, build etc.)
- makes environment setup quickly reproducible, portable
- makes debugging easier (no/ess environment problems)
#### Virtual machine (environment) - VM
- a virtual environment that also virtualizes the hardware and OS layers
 - an abstraction layer that virtualizes the hardware; a package of software, all of its dependencies, virtual OS and hardware specs
##### Configuration manager
- software that automates infrastructure setup (like VM setup), access, application workflows, and other administrative tasks