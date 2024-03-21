# Maven + Red Hat Dependency Analytics Pipeline

This Tekton pipeline uses version 0.1.0 of the [Red Hat Dependency Analytics] task to provide vulnerability and compliance analysis for a hello world Maven application.  This task has been configured
to turn off authentication to the Snyk vulnerability data provider:
```
      env:
        - name: API_SNYK_DISABLED
          value: "true"
```

The pipeline was built on top of the [Tekton Tutorial] which uses the [Tekton Tutorial Greeter] example application.

[Red Hat Dependency Analytics]: https://hub.tekton.dev/tekton/task/redhat-dependency-analytics
[Tekton Tutorial]: https://github.com/redhat-scholars/tekton-tutorial/blob/master/workspaces/greeter-app-deploy.yaml
[Tekton Tutorial Greeter]: https://github.com/redhat-scholars/tekton-tutorial-greeter

