# million-dollar-k8s

# ** This documentation is currently incomplete. Once there is a more solid
direction for how everything is organized, the documentation will be updated to
reflect this organization.
# Function:
This repo is intended to give visibility into the healthy of Kubernetes clusters (i.e. the
million dollar problem) using the
Elastic stack and Prometheus (in the future). Useful visualizations, a 
paired with an alert.
# Requirements:
* metricbeat configured to talk to an ElasticSearch cluster
* kube-state-metrics deployed within the Kubernetes cluster
* metrics-server deployed within the Kubernetes cluster
* A Slack WebHook configured within ElasticSearch
* Several additional fields on documents created by metricbeat
* Prometheus enabled on the Kubernetes cluster (WIP)

Included in this repo are deployments for metricbeat, filebeat,
kube-state-metrics, metrics-server, prometheus under the prerequisites
directory if needed. *beats configuration is the most important! Most if not all
other Elastic work in this repo depends on it (additional fields)
