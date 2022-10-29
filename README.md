yaml```
nexus/Chart.yaml
helm package nexus -d charts
helm repo index charts
.
|-- README.md
|-- archive
|-- charts
|   |-- index.yaml
|   |-- nexus-42.0.1.tgz
|   `-- sonarqube-6.0.0+403.tgz
|-- nexus
|   |-- Chart.yaml
|   |-- LICENSE
|   |-- README.md
|   |-- templates
|   |-- test-output.xml
|   |-- tests
|   `-- values.yaml
`-- sonarqube
    |-- CHANGELOG.md
    |-- Chart.lock
    |-- Chart.yaml
    |-- README.md
    |-- charts
    |-- templates
    |-- values.schema.json
    `-- values.yaml
```
