# Extended Contributing Guidelines

This requirements are built on top of [the base contributing guidelines](./CONTRIBUTING.md).

Even though they may not be followed perfectly in every project all the time, in a world where a perfect project exists everything here is followed.

## Committing Code

Use [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) for your commit messages. Don't think too hard about it though, just keep your commits small, that will make it easy to pick the right message.

## Development cycle 

Use [https://trunkbaseddevelopment.com/](trunk based development) for working on the project. You are free to request reviews at any time, but any branch should not live longer than a week.

## Testing

Write the test first then the implementiatiion

### Unit Testing

Test every function that has an if or writes data to persistent storage. Testing other functions usually is overhead since they will be covered by the end-to-end tests anyways.

### End To End Testing

Write gherkin files (even if the tests are not yet set up) and execute them with behat.

## Dont dry yourself

Value the ease of communicating logic quickly over the dry principle. 
