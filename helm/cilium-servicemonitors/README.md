# cilium-servicemonitors

Cilium ServiceMonitors

![Version: 0.2.0](https://img.shields.io/badge/Version-0.2.0-informational?style=flat-square)
![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square)
![AppVersion: 0.2.0](https://img.shields.io/badge/AppVersion-0.2.0-informational?style=flat-square)

**Homepage:** <https://github.com/giantswarm/cilium-servicemonitors-app>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| cluster.kubernetes.clusterDomain | string | `"cluster.local"` |  |
| disabled | bool | `false` |  |
| releaseLabel | bool | `false` |  |
| agent.enabled | bool | `true` |  |
| agent.scrapeInterval | string | `"60s"` |  |
| agent.relabelings[0].sourceLabels[0] | string | `"__meta_kubernetes_pod_node_name"` |  |
| agent.relabelings[0].targetLabel | string | `"node"` |  |
| agent.relabelings[0].replacement | string | `"${1}"` |  |
| agent.metricRelabelings[0].sourceLabels[0] | string | `"__name__"` |  |
| agent.metricRelabelings[0].regex | string | `"cilium_(node_connectivity_latency_seconds|node_connectivity_status|k8s_client_api_latency_time_seconds_bucket|agent_api_process_time_seconds_bucket|policy_regeneration_time_stats_seconds_bucket)"` |  |
| agent.metricRelabelings[0].action | string | `"drop"` |  |
| hubble.enabled | bool | `true` |  |
| hubble.scrapeInterval | string | `"60s"` |  |
| hubble.relabelings[0].sourceLabels[0] | string | `"__meta_kubernetes_pod_node_name"` |  |
| hubble.relabelings[0].targetLabel | string | `"node"` |  |
| hubble.relabelings[0].replacement | string | `"${1}"` |  |
| hubble.metricRelabelings | list | `[]` |  |
| operator.enabled | bool | `true` |  |
| operator.scrapeInterval | string | `"60s"` |  |
| operator.relabelings | list | `[]` |  |
| operator.metricRelabelings | list | `[]` |  |
