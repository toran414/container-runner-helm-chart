# Container Agent Helm Chart Changelog

This is the Container Agent Helm Chart changelog

# 101.0.20

- [#41](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/41) Expose log settings for container-agent in the values file.

# 101.0.19

- [#39](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/39) fix clusterrole indentation when adding rules #39

# 101.0.18

- [#38](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/38) Add option to set the garbage collection (GC) period to tune how quickly failed Pods are removed.

# 101.0.17

- [#37](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/37) Update the values file and README for the SSH reruns [open preview](https://circleci.com/docs/container-runner-installation/#enable-rerun-job-with-ssh).

# 101.0.16

- [#36](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/36) Add field to set arbitrary environment variables for container-agent

# 101.0.15

- [#34](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/34) [PRERELEASE] Add an option to specify an existing GatewayClass for SSH reruns

# 101.0.14

- [#35](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/35) [PRERELEASE] Support the namespace field in ParametersReference for the SSH reruns GatewayClass

# 101.0.13

- [#33](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/33) [PRERELEASE] Add finalizer on GatewayClass to ensure proper cleanup

# 101.0.12

- [#31](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/31) Fixed PDB to reference the right variable

# 101.0.11

- [#16](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/16) [PRERELEASE] Support SSH reruns

# 101.0.10

- [#29](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/29) Added Proxy env support

# 101.0.8

- [#20](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/20) Use the current major release `3` tag instead of the rolling `edge` tag for the logging-collector image

# 101.0.7

- Update README with new parameters & add some documentation links to `values.yaml`

# 101.0.6

- Add `digest` paramater in `image` settings
- Add `forceUpdate` option

# 101.0.5

- Fix `logging-collector` RBAC permissions
- Annotate the correct service account name on the `logging-collector-token` secret

# 101.0.4

Simplify rbac implementation, avoid cluster role collision

# 101.0.3

Revert breaking change in 101.2 that required a list for roles and cluster roles
                                       
# 101.0.2

Break RBAC template into two seperate template files, cleanup whitespace

# 101.0.1

Remove command from agent pod spec to use command specified in the image Dockerfile

# 101.0.0

Update default image repository to `circleci/runner-agent`

## 100.0.1

Set custom service account even if `create` is set to `false` ([PR #5](https://github.com/CircleCI-Public/container-runner-helm-chart/pull/5))

## 100.0.0 

Initial release of helm chart
