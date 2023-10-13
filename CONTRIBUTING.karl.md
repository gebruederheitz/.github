# Extended Contributing Guidelines

This requirements are built on top of [the base contributing guidelines](./CONTRIBUTING.md).

Even though they may not be followed perfectly in every project all the time, in a world where a perfect project exists everything here is followed.

These guidelines are for the projects lead by Karl and are not rules for the organization.

## Committing Code

Use [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) for your commit messages. Don't think too hard about it though, just keep your commits small, that will make it easy to pick the right message.

## Development cycle 

Use [trunk based development](https://trunkbaseddevelopment.com) for working on the project. You are free to request reviews at any time, but any branch should not live longer than a week. Feel free to use the app environment as a feature flag.

## Testing

Write the test first then the implementiatiion

### Unit Testing

Test every function that has an if or writes data to persistent storage. Testing other functions usually is overhead since they will be covered by the end-to-end tests anyways.

### End To End Testing

Write gherkin files (even if the tests are not yet set up) and execute them with behat.

## Dont dry yourself

Value the ease of communicating logic quickly over the dry principle. 

## Deployments

All deployments are the git archive at the latest head of the trunk. Supporting assets like css might get built in CI for deployment. Secrets are set as part of the deployment process.

## Make it repetable

Value config files in the vcs over backend settings. Value scripts over ssh interaction. Value repeatability over speed.

# 2 Factors??? We need moar!!!

Joking aside, follow the guidelines on https://12factor.net/ to produce a robust application.
