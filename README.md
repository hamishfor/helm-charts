# helm-charts

My personal helm charts, this repo is a collection of charts for my app of apps deployment in argo. It relies heavily on my argo and k8s install, which is managed via ansible in my ansible repo, and my values repository which are both private.

To create a release, bump the `version` in any chart's `Chart.yaml` under the `charts/` directory and push to `main`. The release workflow will automatically package and publish the chart to `gh-pages`. Renovate will auto-bump chart versions when dependencies update. Don't forget to run `helm-docs`.