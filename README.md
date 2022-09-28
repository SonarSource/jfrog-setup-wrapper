# jfrog-setup-wrapper

ease the usage of jfrog/jfrog-setup within Sonar.

## usage

this wrapper will select <https://repox.jfrog.io> automatically.

### providing a token

```yaml
- name: Setup JFrog
  uses: SonarSource/jfrog-setup-wrapper@ref...
  with:
    jfrogAccessToken: secret...
```

### authenticate via vault

Use the suffix configured as part of the artifactory vault role.

```yaml
- name: Setup JFrog
  uses: SonarSource/jfrog-setup-wrapper@ref...
  with:
    artifactoryRoleSuffix: private-reader
```

### advanced

[see action inputs](action.yaml)
