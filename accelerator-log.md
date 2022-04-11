# Accelerator Log

## Options
```json
{
  "deploymentType" : "workload",
  "gitbranch" : "main",
  "giturl" : "https://github.com/TanzuDK/python-test.git",
  "projectName" : "python-test"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ engine.transformations[0].merge (Chain)
┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┏ engine.transformations[0].merge.transformations[0] (Merge)
┃ ┃ ┃  Info Running Merge(YTT, Combo)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0] (YTT)
┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"deploymentType":"workload","gitbranch":"main","artifactVersion":"0.0.1-beta","artifactId":"python-test","giturl":"https://github.com/TanzuDK/python-test.git","projectName":"python-test"}
┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input10544137550306904857, --data-values-file, /tmp/accelerator-options11842691470755425826.json, --output-files, /tmp/ytt-output17121374564307085051]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[1].include (Include)
┃ ┃ ┃ ┃  Info Will include [**/*.py, **/*.txt, **/*.sh, Procfile]
┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.py, **/*.txt, **/*.sh, Procfile] -> excluded
┃ ┃ ┃ ┃ Debug Procfile matched [**/*.py, **/*.txt, **/*.sh, Procfile] -> included
┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.py, **/*.txt, **/*.sh, Procfile] -> excluded
┃ ┃ ┃ ┃ Debug accelerator-log.md didn't match [**/*.py, **/*.txt, **/*.sh, Procfile] -> excluded
┃ ┃ ┃ ┃ Debug app.py matched [**/*.py, **/*.txt, **/*.sh, Procfile] -> included
┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/*.py, **/*.txt, **/*.sh, Procfile] -> excluded
┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [**/*.py, **/*.txt, **/*.sh, Procfile] -> excluded
┃ ┃ ┃ ┃ Debug images/python.png didn't match [**/*.py, **/*.txt, **/*.sh, Procfile] -> excluded
┃ ┃ ┃ ┃ Debug k8s-resource.yaml didn't match [**/*.py, **/*.txt, **/*.sh, Procfile] -> excluded
┃ ┃ ┃ ┃ Debug kubernetes/deployment.yaml didn't match [**/*.py, **/*.txt, **/*.sh, Procfile] -> excluded
┃ ┃ ┃ ┃ Debug requirements.txt matched [**/*.py, **/*.txt, **/*.sh, Procfile] -> included
┃ ┃ ┃ ┃ Debug setup.sh matched [**/*.py, **/*.txt, **/*.sh, Procfile] -> included
┃ ┃ ┗ ┗ Debug values.yml didn't match [**/*.py, **/*.txt, **/*.sh, Procfile] -> excluded
┃ ┃ ┏ engine.transformations[0].merge.transformations[1] (UniquePath)
┃ ┗ ┗ Debug Multiple representations for path 'requirements.txt', will use the one appearing last 
┗ ╺ engine.transformations[1] (UniquePath)
```
