# Maven Puzzlers

This repository contains a set of Maven Puzzlers that are designed to test your knowledge of Maven. Each puzzler is a
small Maven project that contains a `pom.xml` file with a problem. The puzzlers are in their own branch.
The problems all focus on duplicate dependencies, dependency resolution, and Maven's dependency mediation.

These are the branches:
* 01-duplicates
* 02-duplicate-in-transitive
* 03-dependency-management
* 04-direct-and-dependency-management
* 05-duplicate-from-transitive-only

To solve a puzzler, check out the branch and try to determine which version of Guava maven will choose.
Then run `./mvnw dependency:tree -Dincludes=com.google.guava:guava` to see if you were correct.
You can add the `-Dverbose` flag to the command to see which versions where omitted and/or overridden.