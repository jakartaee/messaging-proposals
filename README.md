# How to submit a proposal

A proposal should be associated with an existing use case issue that describes the use case and description of the problem to solve.

To submit a proposal, create a pull request and mention the associated use case issue in the description. Create a new directory for the proposal as described below.

Here’s the concept in practice:

* Every proposal gets a directory and readme and things can be merged pretty much immediately
* The README would describe the idea and motivation
* The src/main/java would contain the proposed API classes
* The src/test/java might contain any associated TCK tests or mock usage
* If someone likes an idea but imagines it slightly differently they can copy the dir and tweak it

More detailed information here: [The Proposals repository](https://github.com/eclipse-ee4j/jms-api/wiki/The-Proposals-repository)