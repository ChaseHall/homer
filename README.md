# Homer
A dead simple static **HOM**epage for your serv**ER** to keep your services on hand, from a simple `yaml` configuration file.

If you need authentication support, you're on your own (it can be secured using a web server auth module or exposing it only through a VPN network / SSH tunnel, ...)

![screenshot](https://git.chasehall.net/Chase/homer/raw/branch/master/screenshot.png)

**How to build / install it? Where is the webpack config?**
There is no build system (😱), use it like that! It's meant to be stupid simple & zero maintenance required. just copy the static files somewhere, and visit the `index.html`.


## configuration

Title, icons, links, colors, and services can be configured in the `config.yml` file, using [yaml](http://yaml.org/) format.


```yaml
---
# Services
# First level array represent a group.
# Leave only a "items" key if not using group (group name, icon & tagstyle are optional, section separation will not be displayed).
services:
  - name: "Services"
    icon: []
    items:
      - name: "qBittorrent"
        logo: "assets/tools/qbit.png"
        subtitle: "Admin UI for Torrents"
        tag: ""
        url: "http://127.0.0.1:8080"
  - name: "Plex"
    icon: []
    items:
      - name: "Plex"
        logo: "assets/tools/plex.png"
        subtitle: "Plex Media Server Frontend"
        tag: ""
        url: "http://127.0.0.1:32400/web/index.html"
      - name: "Sonarr"
        logo: "assets/tools/sonarr.jpg"
        subtitle: "Automatically download TV Shows for Plex"
        tag: ""
        url: "http://localhost:8989/"
      - name: "Radarr"
        logo: "assets/tools/radarr.png"
        subtitle: "Automatically download Movies for Plex"
        tag: ""
        url: "http://localhost:7878/"
      - name: "Jackett"
        logo: "assets/tools/jackett.png"
        subtitle: "Manage trackers for Sonarr + Radarr"
        tag: ""
        url: "http://localhost:9117/"
```
