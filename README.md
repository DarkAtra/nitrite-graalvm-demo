# nitrite-graalvm-demo

Requires installing this PR branch locally: https://github.com/nitrite/nitrite-java/pull/995
This can be done by cloning the branch and then running: `mvn clean install -Dgpg.skip=true`

The [following directory](src/test/java/org/dizitart/nitrite/demo/repository) contains a few tests that
perform read and write operations from and to a nitrite database. These tests can be run:

* using the JVM: `mvn clean verify`
* using the native image via GraalVM: `mvn clean verify -PnativeTest`

See [the Person class](src/test/java/org/dizitart/nitrite/demo/repository/model/Person.java) for details regarding
native hints.
