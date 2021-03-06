# Dapr demos

Collection of personal [Dapr](https://dapr.io) demos.

> Note, some of these demos require latest version of Dapr, Ingress gateway, Observability components, or cluster-local Redis and Mongo services. To create Kubernates cluster with all these components on AKS, or quickly configure an existing cluster, consider the [Dapr Cluster Setup](./setup) utility.


* Bindings
  * [Scheduling using cron](./cron-binding) - Using scheduler to execute service 
  * [Tweet stream](./pipeline/tweet-provider) - Subscribing to a Twitter even stream and publishing to a pub/sub topic
  * [State change handler](./state-change-handler) - RethinkDB state changes streamed into topic
* Eventing
  * [gRPC event subscriber](./grpc-event-subscriber) - Subscribing to topic and processing its events using gRPC service
  * [HTTP event subscriber](./http-event-subscriber) - Subscribing to topic and processing its events using HTTP service
* Services 
  * [gRPC echo service](./grpc-echo-service) - gRPC service invocation example
  * [HTTP echo service](./http-echo-service) - HTTP service invocation example
  * [Sentiment Scorer](./pipeline/sentiment-scorer) - Sentiment scoring serving backed by Azure Cognitive Service 
* Integrations
  * [Dapr API in ACI](./dapr-aci) - Dapr components as microservices 
  * [Dapr as component API](./component-api) - Zero-app Dapr instance used as a component API server 
  * [Dapr with APIM](./apim-gateway) - Dapr API using Azure API Management self-hosted gateway
* Solutions
  * [Order cancellation](./order-cancellation) - multiple Dapr service integrations with observability
  * [Pipeline](./pipeline) - Demos combining Twitter binding, Sentiment scoring, Multi Pub/Sub Processor, and WebSocket Viewer app
  * [Fan-out](./fan-out) - Single message source "broadcasted" to multiple, configurable targets (e.g. Redis PubSub, HTTP, gRPC)
* Templates
  * [Dapr gRPC Service](https://github.com/mchmarny/dapr-grpc-service-template) - gRPC service template
  * [Dapr HTTP Event Subscriber](https://github.com/mchmarny/dapr-http-event-subscriber-template) - Event subscriber HTTP service template
  * [Dapr gRPC Event Subscriber](https://github.com/mchmarny/dapr-grpc-event-subscriber-template) - Event subscriber gRPC service template 
  * [dapr-http-cron-handler](https://github.com/mchmarny/dapr-http-cron-handler-template) - Scheduled service development template

## Disclaimer

This is my personal project and it does not represent my employer. While I do my best to ensure that everything works, I take no responsibility for issues caused by this code.

## License

This software is released under the [MIT](./LICENSE)
