## Environment managers
### Docker 
- container management system
- open source
- more about operating a single container, but can run many via docker-compose or docker swarm
- meant to run on a single node (device)
### kubernetes
- container management system
- open source
- includes pipeline automation
- more about orchestrating multiple containers (ex. when app needs many)
- meant to run across a cluster of nodes
- can run Docker (and similar) inside of it
### Vagrant
- virtual (machine) environment management system
- open source
- can run other managers (different abstraction layer - docker but for VM/entire system, not a container)
## Configuration managers


https://www.upguard.com/articles/ansible-puppet

https://en.wikipedia.org/wiki/Software_configuration_management
* Ansible
* Puppet
* Salt / SaltStack
* Chef
## Virtual machines
* Oracle VirtualBox
* VMware Workstation
* Amazon Elastic Compute Cloud (AWS EC2)
## Build automation
https://en.wikipedia.org/wiki/List_of_build_automation_software
#### Apache Maven
- mostly Java, but also C#, Ruby, Scala
- manages build, job order and dependencies
- XML config files
- linear progression of build phases
#### Gradle
- manages build, task order and dependencies
- Groovy-based DSL (Domain Specific Language, own way to write scripts) config files
- graph-based progression of build tasks
#### Apache Ant
- mostly Java, but also C or C++
- build tool, library and command-line level
- does not OOTB manage dependencies
- can automate assembling, compiling, testing and running apps
- XML config files
## Continuous integration tools
https://en.wikipedia.org/wiki/Comparison_of_continuous_integration_software
* Jenkins
* GitLab
* Travis CI
* CircleCI
* Atlassian Bamboo
* Azure DevOps
* AWS CodePipeline
