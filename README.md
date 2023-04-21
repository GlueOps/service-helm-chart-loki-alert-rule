# loki-alert-rule

![Version: 0.1.0-antonio-alpha3](https://img.shields.io/badge/Version-0.1.0--antonio--alpha3-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square)

This chart enables creation of a loki alert based on a LogQL query.

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| description | string | `"This is the default alert description. Please change this to be more useful."` | Description of the alert. Make this informative to the responding team(s) know what this alert is for. |
| duration | string | `"10m"` | Amount of time for the LogQL expression to be true before an alert gets fired. |
| expr | string | `"vector(0)"` | LogQL Expression |
| labels.component | string | `"nil"` | Name of component. Ex. backend, frontend, authentication, database, search. |
| labels.team | string | `"nil"` | Team name that will react to any alerts |
