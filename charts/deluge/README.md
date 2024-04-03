# deluge

![Version: 5.4.2](https://img.shields.io/badge/Version-5.4.2-informational?style=flat-square) ![AppVersion: v2.0.3-2201906121747](https://img.shields.io/badge/AppVersion-v2.0.3--2201906121747-informational?style=flat-square)

Deluge is a torrent download client

**Homepage:** <https://github.com/k8s-at-home/charts/tree/master/charts/stable/deluge>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| mcmarkj | <mark@markmcw.uk> |  |

## Source Code

* <https://hub.docker.com/r/linuxserver/deluge/>
* <https://deluge-torrent.org/>

## Requirements

Kubernetes: `>=1.16.0-0`

| Repository | Name | Version |
|------------|------|---------|
| https://library-charts.k8s-at-home.com | common | 4.5.2 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| env | object | See below | environment variables. See more environment variables in the [deluge documentation](https://github.com/linuxserver/docker-deluge#parameters). |
| env.DELUGE_LOGLEVEL | string | `"error"` | Set the loglevel output when running Deluge |
| env.PGID | string | `"1000"` | Specify the group ID the application will run as |
| env.PUID | string | `"1000"` | Specify the user ID the application will run as |
| env.TZ | string | `"Europe/London"` | Set the container timezone |
| image.pullPolicy | string | `"IfNotPresent"` | image pull policy |
| image.repository | string | `"linuxserver/deluge"` | image repository |
| image.tag | string | `"2.1.1-r8-ls262"` | image tag |
| ingress.main | object | See values.yaml | Enable and configure ingress settings for the chart under this key. |
| persistence | object | See values.yaml | Configure persistence settings for the chart under this key. |
| service | object | See values.yaml | Configures service settings for the chart. |

