# AWS Parameter Store Orb
Easily load AWS parameter store keys into your CircleCI environment.

Orbs are reusable [commands](https://circleci.com/docs/2.0/reusing-config/#authoring-reusable-commands), [executors](https://circleci.com/docs/2.0/reusing-config/#authoring-reusable-executors), and [jobs](https://circleci.com/docs/2.0/reusing-config/#jobs-defined-in-an-orb) (as well as [usage examples](https://github.com/CircleCI-Public/config-preview-sdk/blob/v2.1/docs/usage-examples.md))—snippets of CircleCI configuration—that can be shared across teams and projects. See [CircleCI Orbs](https://circleci.com/orbs), [Explore Orbs](https://circleci.com/orbs/registry), [Creating Orbs](https://circleci.com/docs/2.0/creating-orbs), and [Using Orbs](https://circleci.com/docs/2.0/using-orbs) for further information.

Orb registry: https://circleci.com/orbs/registry/orb/circleci/aws-parameter-store

## How to publish a new version

You need to have the `circleci` utility installed first:

```bash
brew install circleci
```

Then, define a new version to be published. From the `src/` folder, run the following commands:

```bash
circleci orb pack . > ~/Downloads/orb.yml
circleci orb publish ~/Downloads/orb.yml zookal/aws-parameter-store@1.0.MY_NEW_VERSION_NUMBER
```