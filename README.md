# Homer [![GitHub stars](https://img.shields.io/github/stars/ChaseHall/homer)](https://github.com/ChaseHall/homer/stargazers)
A dead simple static **HOM**epage for your serv**ER** to keep your services on hand, from a simple `yaml` configuration file.

If you need authentication support, you're on your own.

![screenshot](https://i.imgur.com/LUu52eR.png)

**How to use?**
Simply copy the files to a directory on your web server, and visit `index.html`.
**Note: This will not work directly over file:// protocol.**


## Configuration

Title, icons, links, colors, and services can be configured in the `config.yml` file, using [yaml](http://yaml.org/) format.


```yaml
---
services:
  - name: "Section 1"
    icon: []
    items:
      - name: "Service 1"
        logo: "https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/Flat_tick_icon.svg/1200px-Flat_tick_icon.svg.png"
        subtitle: "Lorem ipsum dolor sit amet."
        tag: ""
        url: "https://domain.tld"
      - name: "Service 2"
        logo: "https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/Flat_tick_icon.svg/1200px-Flat_tick_icon.svg.png"
        subtitle: "Lorem ipsum dolor sit amet."
        tag: ""
        url: "https://subdomain.domain.tld"
      - name: "Service 3"
        logo: "https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/Flat_tick_icon.svg/1200px-Flat_tick_icon.svg.png"
        subtitle: "Lorem ipsum dolor sit amet."
        tag: ""
        url: "https://sub.domain.tld/page"
  - name: "Plex"
    icon: []
    items:
      - name: "Service 1"
        logo: "https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/Flat_tick_icon.svg/1200px-Flat_tick_icon.svg.png"
        subtitle: "Lorem ipsum dolor sit amet."
        tag: ""
        url: "https://domain.tld"
      - name: "Service 2"
        logo: "https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/Flat_tick_icon.svg/1200px-Flat_tick_icon.svg.png"
        subtitle: "Lorem ipsum dolor sit amet."
        tag: ""
        url: "https://subdomain.domain.tld"
      - name: "Service 3"
        logo: "https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/Flat_tick_icon.svg/1200px-Flat_tick_icon.svg.png"
        subtitle: "Lorem ipsum dolor sit amet."
        tag: ""
        url: "https://sub.domain.tld/page"
```
