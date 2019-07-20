# Layout/Function
prerequisites/elastic-stack/
├── 00_namespace.yaml - the namespace where all kubernetes objects will live in.
Needs to be created first
├── elastic-cloud-auth.yml - shared *beats configuration
├── elastic-cloud-auth.yml - shared *beats configuration
├── elastic-site-data.yml - k8s cluster and site information for documents
├── metricbeat
│   ├── metricbeat-daemonset-configmap.yaml
│   ├── metricbeat-daemonset.yaml
│   ├── metricbeat-deployment-configmap.yaml
│   ├── metricbeat-deployment.yaml
│   ├── metricbeat-role-binding.yaml
│   ├── metricbeat-role.yaml
│   └── metricbeat-service-account.yaml
├── metricbeat-7-template.json - an index template and alias for easier
searching
└── README.md - this file
