# seedwing-java-example

Example Java project integrating with Seedwing.

This example consists the following:

* A [quarkus](java) Java application with the CycloneDX maven plugin enabled.
* A [GitHub Actions Workflow](.github/workflows/ci.yaml#L15) contains an example CI pipeline that builds the SBOM and performs policy checks using `seedwing-policy-cli`.
* An [alternative workflow](.github/workflows/proxy-ci.yaml) that configures maven to fetch the app's dependencies through the [`seedwing-proxy`](https://github.com/seedwing-io/seedwing-proxy)
* A [set of policies](policies/) that are applied at different stages in the CI pipelines.
