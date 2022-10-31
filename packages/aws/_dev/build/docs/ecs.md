# Amazon ECS

The Amazon ECS integration allows you to monitor [Amazon Elastic Container Service (Amazon ECS)](https://aws.amazon.com/ecs/)—a managed container orchestration service.

Use the Amazon ECS integration to collect metrics related to your ECS instances. Then visualize that data in Kibana, create alerts to notify you if something goes wrong, and reference the metrics when troubleshooting an issue.

For example, you could use this data to track Amazon ECS CPU and memory utilization. Then you can alert when utilization for an instance crosses a predefined threshold.

## Data streams

The Amazon ECS integration collects one type of data: metrics.

**Metrics** give you insight into the state of Amazon ECS.
The metrics collected by the Amazon ECS integration include CPU utilization, CPU reservation, memory reservation, memory utilization, and more. See more details in the [Metrics reference](#metrics-reference)

## Requirements

You need Elasticsearch for storing and searching your data and Kibana for visualizing and managing it.
You can use our hosted Elasticsearch Service on Elastic Cloud, which is recommended, or self-manage the Elastic Stack on your own hardware.

Before using any AWS integration you will need:

* **AWS Credentials** to connect with your AWS account.
* **AWS Permissions** to make sure the user you're using to connect has permission to share the relevant data.

For more details about these requirements, see the **AWS** integration documentation.

## Setup

Use this integration if you only need to collect data from the Amazon ECS service.

If you want to collect data from two or more AWS services, consider using the **AWS** integration.
When you configure the AWS integration, you can collect data from as many AWS services as you'd like.

For step-by-step instructions on how to set up an integration, see the
{{ url "getting-started-observability" "Getting started" }} guide.

## Metrics reference

{{event "ecs_metrics"}}

{{fields "ecs_metrics"}}