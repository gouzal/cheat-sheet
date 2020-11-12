# sonar-project.properties
## A simple SonarQube config for generic Java projects   
``` YAML
# must be unique in a given SonarQube instance
sonar.projectKey=project:id

# --- optional properties ---

# defaults to project key
sonar.projectName=My project
# defaults to 'not provided'
sonar.projectVersion=1.0
 
# Path is relative to the sonar-project.properties file. Defaults to .
sonar.sources=.

sonar.exclusions=**/*Test*.java,**/jalo/**,**/gensrc/**
sonar.inclusions=**/*.java
sonar.java.binaries=**/classes/**

# Encoding of the source code. Default is default system encoding
#sonar.sourceEncoding=UTF-8
```
