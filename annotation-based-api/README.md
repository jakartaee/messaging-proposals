# Annotation-based consumer and client API

The idea is to introduce an alternative API for consuming and sending messages that is easy to work with and uses the full potential of annotations, interfaces and generation of proxies wherever possible.

There are 2 parts to it:

* The consumer part (which replaces or improves MDBs), described in https://github.com/eclipse-ee4j/jms-api/issues/243
* The client part (which replaces or improves the JMSProducer/JMSConsumer API), described in https://github.com/eclipse-ee4j/jms-api/issues/249

If possible, each proposal should address both the consumer and client part because it's expected there some parity between them, e.g. the API may reuse the same annotations for both the consumer (server) and the client part.

The client part can be then separated to producer client and consumer client parts, each of them can be addressed separately or not at all (e.g. a proposal can only address the message producer/sender client part). 

