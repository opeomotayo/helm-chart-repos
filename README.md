
 5326  mv charts/*.tgz archive
 5327  lc charts
 5328  ls charts
 5329  helm package nexus -d charts
 5330  helm package sonarqube -d charts
 5331  helm repo index charts
 5332  cat charts/index.yaml
 5333  git add -A
 5334  git commit -am "testing nexus chart"
 5335  show system resources
 5336  git push
 5337  helm repo update
 5338  helm install -n sonarqube sonarqube sonarqube
 5339  helm install -n nexus nexus nexus

nexus/Chart.yaml
helm package nexus -d charts
helm repo index charts
.
|-- README.md
|-- archive
|-- charts
|   |-- index.yaml
|   |-- nexus-42.0.1.tgz
|   -- sonarqube-6.0.0+403.tgz
|-- nexus
|   |-- Chart.yaml
|   |-- LICENSE
|   |-- README.md
|   |-- templates
|   |-- test-output.xml
|   |-- tests
|   -- values.yaml
-- sonarqube
    |-- CHANGELOG.md
    |-- Chart.lock
    |-- Chart.yaml
    |-- README.md
    |-- charts
    |-- templates
    |-- values.schema.json
    -- values.yaml

