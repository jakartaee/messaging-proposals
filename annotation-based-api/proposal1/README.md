# Annotation-based consumer and client API - proposal 1

This proposal is based on the proposals in the https://github.com/tomitribe/jms-proposals repository.

The gist of the proposal:

* The consumer part is exemplified in the `NotificationsListener` and `BuildAndNotify` classes, which are annotated by `@MessageConsumer` and their method annotated by `@TopicListener` or `QueueListener` annotations
* The client part is exemplified in the `BuildAndNotify` class, which uses the `MessagingClientBuilder` builder to build an implementation of an interface (`NotificationsClient`). The `NotificationsClient` is a client interface which defines that how the client object should be built. Each method and its parameters are annotated to specify the target queue or topic and how to convert arguments to a message.