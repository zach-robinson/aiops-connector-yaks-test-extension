# AIOps-Connector-Yaks-Test-Extension

## Usage

To use add these options to the `yaks-config.yaml` file in your test directory:

```yaml
config:
  runtime:
    cucumber:
      glue:
        - "org.citrusframework.yaks"
        - "com.ibm.aiops.connectors.steps"
    settings:
      repositories:
        - id: "central"
          name: "Maven Central"
          url: "https://repo.maven.apache.org/maven2/"
        - id: "jitpack.io"
          name: "JitPack Repository"
          url: "https://jitpack.io"
      dependencies:
        - groupId: com.github.zach-robinson
          artifactId: aiops-connector-yaks-test-extension
          version: 0.0.13
```