# pupperware-party

A pupperware based load and performance tester for Puppet 6

## Getting Started

This section will need to be fleshed out, once the MVP is available. In this section, there will be a a way to get started quickly, for those who don't want to read all the documentation.

### Prerequisites

You will need an existing puppetserver, running at least version 6. You will also need to have a Docker Engine available.

Additionally, you will need your puppet master to be able to autosign the certificates for the nodes created by this process.
Your puppet code will also need to be set up in a way that nodes can be automatically classified - use of a naming scheme, or facts that can be placed at provision time for example.

### Installion

Installation steps will go here, once those have been determined.

## ToDo

* All the things
* Flesh out the README better
  * Add Usage section
* Define MVP for inital release
* Decide language to use for generating yaml for dockerfiles/composefile
* Determine what needs to go into the dockerfiles/composefile
* Add adr for licensing choice
* Decide and define initial supported naming scheme for nodes
* Decide name for test nodes
* Decide metrics to be gathered during tests
* Create a logo
* Decide on a language/format for config files
  * JSON?
  * Hocon?
  * YAML?
  * raw key value pairs?
* Determine what options can be configured via the config files
* Determine where config files should live and in what order they should be parsed


## Context

This section looks at why I started this project and what I hope to be able to accomplish with it.

### Backstory

Testing is an important part of the software lifecycle, and this is true even for infrastructure as code. Web applications are often load tested to ensure that they are able to work at "web scale", and this sort of testing is also useful for performance tuning. For infrastructure as code. Companies often experience periods of rapid growth, and it can be difficult to know when or how to scale your infrastructure as code setup. Do you just need to throw more ram and processors into your master? Or do you need to add more compile masters? Or can you just adjust the configuration? Performance and load testing can help you make informed decisions.

### Goals

The goal of this project is to provide a simple way to perform load and performance testing to be able to make informed decisions about scaling a puppet stack and beable to tune your stack to be able to get the most out of your existing hardware.

## Contributing

Information on contributing will go here. This will likely involve a link to the issues section and some guide lines around pull requests and coding style and the like.

## Versioning

We use [SemVer](http://semver.org) for versioning. For versions available, please see the [tags on this repository](https://github.com//llowder/pupperware-party/tags).

## Authors

* **Lee "FriedBob" Lowder** - **Initial Author** - [llowder](https://github.com/llowder)

## License

This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) for details.

## Acknowledgements

* afisher for inspiring the name of this project
* binford2k for inspiting actualyl creating this project
