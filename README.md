# helm-charts

My personal helm charts, this repo is a collection of charts for my app of apps deployment in argo. It relies heavily on my argo and k8s install, which is managed via ansible in my ansible repo, and my values repository which are both private.

## Publishing to the Helm repo (gh-pages)

The charts are also published as a normal Helm repo for `helm repo add hamishfor https://hamishfor.github.io/helm-charts`. That URL is GitHub Pages serving the `gh-pages` branch, which holds `index.yaml` plus one `.tgz` per chart version.

`.github/workflows/release.yaml` runs on every push to `main`. It packages any chart whose `version` in `Chart.yaml` isn't on `gh-pages` yet, and adds it to the index. Bump `version` when you want a new published release. Already-published versions are never overwritten.

Don't forget to run `helm-docs`; CI fails if the generated READMEs are out of date.
