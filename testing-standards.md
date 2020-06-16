## Testing Standards

### Unit Testing

Each source file should have 100% coverage in unit testing. Additionally, we make use of Travis CI, which is an open-source continuous integration platform that has seamless GitHub integration for projects. More information about the use of Travis CI can be found [here](http://docs.travis-ci.com/user/).

#### Definition
A unit test is defined as a test cooresponding to the function or method level of a class or module. Specifically, a unit test should cover a small and scoped piece of logic. Where unit tests become large or unwieldly, this shows flaws in the design of the method it was designed to test. More specifically, when this occurs, the function or method should be refactored into smaller and more componentized logic.

#### Usage

1. JVM-based Source - JUnit Test Suites
2. NodeJS Server-side JavaScript - Jasmine (```jasmine-node```)
3. User Interface Components - Jasmine + Angular Mocks

Additionally, the acceptance of source code is dependent on the quality of the unit tests associated with it. Tests that are written to only pass, without true logic testing, will be denied based on a quality assessment. Those tests written that do check logic but without complete coverage will also be denied with a request for more robust testing.

### End-Point Testing

While RESTful end-point testing could be considered an integration test, we are specifically defining these tests as an independant activity. This allows for full-coverage tests of the RESTful APIs regardless of their implementaiton (JVM/NodeJS). These end-point tests should cover 100% of the API services and options, to include parameters, HTTP header checks, and formatting where appropriate.

These tests will be conducted using [Frisby.js](http://frisbyjs.com/).

### Integration Testing

All source code interaction should attempt 100% testing coverage. As with unit tests, source-level integration tests should be written for use with TravisCI in mind.

#### Definition

Integration tests verify the interaction between modules in the source code, as well as interactions between the source code and outside dependencies (such as a persistence module to MongoDB). For the use of integration testing, we specify testing only for module interaction as a requirement. Integration tests for infrastructure (such as the use of caches, databases, or other dependencies) are the responsibility of the infrastructure provider for their environment.

#### Usage

1. JVM-based Source - JUnit Test Suites
2. NodeJS Server-side JavaScript - Jasmine (```jasmine-node```)
3. User Interface Components - Jasmine + Angular Mocks

### Infrastructure Testing

It is critical to treat infrastructure like source code: with versioning, version control, and automation. In this respect, infrastructure changes (such as a configuration specific to Nginx or MongoDB) should have an associated test, and be checked in to version control for use.

### User Interface Testing
Since the browser ecosystem is rich and feature-dependent on the provider, Selenium user interface testing will also be in use to provide automated analysis of DOM construction by browser.
