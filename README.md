# Helm Charts
A Helm Chart Repository

If you like the charts, please help to star our repo!

### Quick links
[PreferredAI](https://preferred.ai/)

## Installation
To install this chart repository

```bash
helm repo add preferred-ai https://charts.preferred.ai
```

## Contributing to an Existing Chart

We'd love for you to contribute to an existing Chart that you find provides a useful application or service for Kubernetes. Please read below for more information on how you can contribute Charts.

### Technical Requirements

* All Chart dependencies should also be submitted independently
* Must pass the linter (`helm lint`)
* Must successfully launch with default values (`helm install .`)
    * All pods go to the running state (or NOTES.txt provides further instructions if a required value is missing e.g. [minecraft](https://github.com/helm/charts/blob/master/stable/minecraft/templates/NOTES.txt#L3))
    * All services have at least one endpoint
* Must include source GitHub repositories for images used in the Chart
* Images should not have any major security vulnerabilities
* Must be up-to-date with the latest stable Helm/Kubernetes features
    * Use Deployments in favor of ReplicationControllers
* Should follow Kubernetes best practices
    * Include Health Checks wherever practical
    * Allow configurable [resource requests and limits](http://kubernetes.io/docs/user-guide/compute-resources/#resource-requests-and-limits-of-pod-and-container)
* Provide a method for data persistence (if applicable)
* Support application upgrades
* Allow customization of the application configuration
* Provide a secure default configuration
* Do not leverage alpha features of Kubernetes
* Includes a [NOTES.txt](https://helm.sh/docs/topics/charts/#chart-license-readme-and-notes) explaining how to use the application after install
* Follows [best practices](https://helm.sh/docs/chart_best_practices/)
  (especially for [labels](https://helm.sh/docs/chart_best_practices/labels/)
  and [values](https://helm.sh/docs/chart_best_practices/values/))

### Documentation Requirements

* Must include an in-depth `README.md`, including:
    * Short description of the Chart
    * Any prerequisites or requirements
    * Customization: explaining options in `values.yaml` and their defaults
* Must include a short `NOTES.txt`, including:
    * Any relevant post-installation information for the Chart
    * Instructions on how to access the application or service provided by the Chart

## License
[Apache License 2.0](LICENSE)
