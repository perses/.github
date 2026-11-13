<div align="center">

<a href="https://perses.dev"><img src="https://raw.githubusercontent.com/cncf/artwork/main/projects/perses/icon/color/perses-icon-color.svg" alt="Perses logo" width="120"></a>

# Perses

**An open specification for dashboards.<br>The open dashboard tool for Prometheus and other data sources.**

[Website](https://perses.dev) · [Documentation](https://perses.dev/docs/perses/latest/) · [Live demo](https://demo.perses.dev) · [Slack](https://cloud-native.slack.com/messages/C07KQR95WBE) · [Discussions](https://github.com/perses/perses/discussions)

</div>

## What is Perses?

Perses is first and foremost a dashboard tool to display observability data. It supports all four observability pillars
through Prometheus metrics, Tempo traces, Loki logs and Pyroscope profiles, and many other datasources through plugins.

Beyond that, Perses aims to be:

- **Open**: it defines a standardized dashboard specification, fostering interoperability across observability tools.
- **Extensible**: its plugin-based architecture lets you add new panels, datasources, queries and variables.
- **Embeddable**: npm packages let you integrate Perses panels and dashboards into your own UI.
- **GitOps-friendly**: a CLI, static validation and SDKs in Go and CUE provide a great Dashboard-as-Code experience.
- **Kubernetes-native**: the Perses Operator manages Perses, dashboards and datasources as custom resources.

## Getting started

Explore the [live demo](https://demo.perses.dev), or run Perses locally with Docker:

```bash
docker run --name perses -d -p 127.0.0.1:8080:8080 persesdev/perses
```

Then open <http://localhost:8080> and follow the
[getting started guide](https://perses.dev/docs/perses/latest/getting-started/) to create your first dashboard. Perses
can also be installed with [Homebrew](https://perses.dev/docs/perses/latest/installation/third-party/),
[Helm](https://github.com/perses/helm-charts) or the [Perses Operator](https://github.com/perses/perses-operator).

## Repositories

| Repository                                                     | Description                                                                                     |
|----------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
| [perses](https://github.com/perses/perses)                     | The Perses server and web UI, the `percli` CLI, and the Go and CUE Dashboard-as-Code SDKs.      |
| [plugins](https://github.com/perses/plugins)                   | The core plugins: datasources (Prometheus, Tempo, Loki, Pyroscope...), panels and variables.    |
| [shared](https://github.com/perses/shared)                     | The `@perses-dev/*` UI libraries, to build plugins or embed Perses panels and dashboards.       |
| [spec](https://github.com/perses/spec)                         | The dashboard and datasource specification, available in CUE, Go, Java and TypeScript.          |
| [perses-operator](https://github.com/perses/perses-operator)   | Kubernetes operator to deploy Perses and manage dashboards and datasources as custom resources. |
| [helm-charts](https://github.com/perses/helm-charts)           | Helm charts for Perses and the Perses Operator.                                                 |
| [community-mixins](https://github.com/perses/community-mixins) | Ready-to-use dashboards, alerting rules and recording rules, written with the Go SDK.           |
| [cli-actions](https://github.com/perses/cli-actions)           | GitHub Actions to build, validate, preview and deploy dashboards as code with `percli`.         |
| [mcp-server](https://github.com/perses/mcp-server)             | MCP server that lets LLM hosts interact with Perses.                                            |
| [metrics-usage](https://github.com/perses/metrics-usage)       | Track where metrics are used across dashboards, alerting rules and recording rules.             |
| [promql-builder](https://github.com/perses/promql-builder)     | Go library to build PromQL expressions.                                                         |

## Community

- Chat with us in [#perses-dev](https://cloud-native.slack.com/messages/C07KQR95WBE) on the CNCF Slack
  ([get an invite](https://slack.cncf.io/)).
- Ask questions and share ideas in [GitHub Discussions](https://github.com/perses/perses/discussions).
- Report bugs and request features in the [issue tracker](https://github.com/perses/perses/issues).
- Join the [weekly team meeting](https://perses.dev/docs/perses/latest/contact/#team-meetings), open to everyone.
- Follow us on [X](https://x.com/PersesDev) and [LinkedIn](https://linkedin.com/company/persesdev).

## Contributing

Contributions of all kinds are welcome! Start with the
[contributing guide](https://github.com/perses/perses/blob/main/CONTRIBUTING.md), and have a look at the
[roadmap](https://github.com/perses/perses/blob/main/ROADMAP.md) and the
[governance](https://github.com/perses/perses/blob/main/GOVERNANCE.md) of the project.

Perses follows the [CNCF Code of Conduct](https://github.com/cncf/foundation/blob/main/code-of-conduct.md). To report
a security vulnerability, please follow our [security policy](https://github.com/perses/perses/blob/main/SECURITY.md).

---

<p align="center">
  Perses is a <a href="https://www.cncf.io/">Cloud Native Computing Foundation</a> sandbox project.
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cncf/artwork/main/other/cncf/horizontal/white/cncf-white.svg">
    <img src="https://raw.githubusercontent.com/cncf/artwork/main/other/cncf/horizontal/color/cncf-color.svg" alt="Cloud Native Computing Foundation logo" width="300">
  </picture>
</p>
