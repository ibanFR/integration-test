_# integration-test

Sample Maven project with basic structure for integration testing.

* Uses [Maven Failsafe Plugin](https://maven.apache.org/surefire/maven-failsafe-plugin/) to run integration tests.
* Uses [Exec Maven Plugin](https://www.mojohaus.org/exec-maven-plugin/) to run java programs for setting up and tearing
  down the integration test environment in the Maven pre-integration-test and post-integration-test lifecycle phases.
* The [Maven Site Plugin](https://maven.apache.org/plugins/maven-site-plugin/)  is used to generate a site for the
  project.
* The [Maven Project Info Reports plugin](https://maven.apache.org/plugins/maven-project-info-reports-plugin/index.html)
  is used to generate reports information about the project.

For running integration tests:
`mvn clean verify -P integration-test`

For generating a report use:
`mvn surefire-report:failsafe-report-only`

See generated reports on target/site/failsafe-report.html.

For generating a site for the project use:
`mvn site`

See generated reports on target/site/index.html.
