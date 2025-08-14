# helm-charts

My personal helm charts, this repo is a collection of charts for my app of apps deployment in argo. It relies heavily on my argo and k8s install, which is managed via ansible in my ansible repo, and my values repository which are both private.

To create a release, modify the Chart.yaml in any of the first level sub directories in the charts directory. Don't forget to run `helm-docs`.