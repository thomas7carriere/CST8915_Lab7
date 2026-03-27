# CST8915_Lab7

Videlio link: https://youtu.be/fC_cb19q5Uk

RabbitMQ Questions:

# Question: Whether RabbitMQ is a stateless or stateful application
RabbitMQ is currently deployed in a stateless manner, as it currently has no persistent storage and any state will be lost upon deletion or restart.
# Question: The implications of running RabbitMQ without persistent storage
Without persistent storage, any events that were stored in RabbitMQ will be lost, and consumers will miss the opertunity of operate on the events.
# Question: What happens when the RabbitMQ pod is deleted or restarted
When the pod is deleted AKS will create a new pod, similar to restarting a pod. All state data will be erased.
# Question: Potential solutions to this problem (research-based)
Creating an attached storage resource to enable persistent storage.
# Question: Does using Azure Service Bus solve the issues identified with RabbitMQ Configuration in this Lab?
Yes it would, as Azure Service Bus provides built-in managed persistence.

