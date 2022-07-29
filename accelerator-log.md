# Accelerator Log

## Options
```json
{
  "deploymentType" : "workload",
  "gitbranch" : "main",
  "giturl" : "https://github.com/TanzuDK/uber-data.git",
  "minscale" : "1",
  "projectName" : "uber-data"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(GeneratorValidationTransform, UniquePath)
┃ ┏ ┏ engine.transformations[0].validated (Combo)
┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ engine.transformations[0].validated.merge (Chain)
┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.transformations[0] (Merge)
┃ ┃ ┃ ┃  Info Running Merge(YTT, Combo)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.transformations[0].sources[0] (YTT)
┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"deploymentType":"workload","gitbranch":"main","artifactVersion":"0.0.1-beta","artifactId":"uber-data","giturl":"https://github.com/TanzuDK/uber-data.git","projectName":"uber-data","minscale":"1"}
┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input2445371065606873656, --data-values-file, /tmp/accelerator-options4202615227459607125.json, --output-files, /tmp/ytt-output16706577968839755813]
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.merge.transformations[0].sources[1].include (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore]
┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ Debug Procfile matched [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> excluded
┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> excluded
┃ ┃ ┃ ┃ ┃ Debug accelerator-log.md didn't match [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> excluded
┃ ┃ ┃ ┃ ┃ Debug app.py matched [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> excluded
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> excluded
┃ ┃ ┃ ┃ ┃ Debug images/python.png didn't match [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> excluded
┃ ┃ ┃ ┃ ┃ Debug k8s-resource.yaml didn't match [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> excluded
┃ ┃ ┃ ┃ ┃ Debug requirements.txt matched [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ Debug setup.sh matched [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> included
┃ ┃ ┃ ┃ ┃ Debug todo.txt matched [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> included
┃ ┃ ┃ ┗ ┗ Debug values.yml didn't match [**/*.py, **/*.txt, **/*.sh, Procfile, .gitignore] -> excluded
┃ ┃ ┃ ┏ engine.transformations[0].validated.merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ Debug Multiple representations for path 'requirements.txt', will use the one appearing last 
┃ ┗ ┗ ┗ Debug Multiple representations for path 'todo.txt', will use the one appearing last 
┗ ╺ engine.transformations[1] (UniquePath)
```
