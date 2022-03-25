## Motivation

- run public maintained images with no modifications
- require minimal configuration and setup

## Features

- [Plex](https://plex.tv/) - organizes video, music and photos from personal media libraries and streams them to smart TVs, streaming boxes and mobile devices.
- [Jellyfin](https://jellyfin.org/) - is the volunteer-built media solution that puts you in control of your media.
- [Ombi](https://ombi.io/) - is a self-hosted web application that automatically gives your shared Plex or Emby users the ability to request content by themselves.
- [Sonarr](https://sonarr.tv/) - is a PVR for usenet and bittorrent users. It can monitor multiple RSS feeds for new episodes of your favorite shows and will grab, sort and rename them. It can also be configured to automatically upgrade the quality of files already downloaded when a better quality format becomes available.
- [Radarr](https://radarr.video/) - A fork of Sonarr to work with movies à la Couchpotato.
- [Bazarr](https://www.bazarr.media/) - is a companion application to Sonarr and Radarr that manages and downloads subtitles based on your requirements.
- [Lidarr](https://lidarr.audio/) - is a music collection manager for Usenet and BitTorrent users.
- [NZBHydra2](https://github.com/theotherp/nzbhydra2) - is a meta search application for NZB indexers, the "spiritual successor" to NZBmegasearcH, and an evolution of the original application NZBHydra.
- [Prowlarr](https://github.com/Prowlarr/Prowlarr) - is a indexer manager/proxy built on the popular arr .net/reactjs base stack to integrate with your various PVR apps.
- [Duplicati](https://www.duplicati.com/) - Free backup software to store encrypted backups online.
- [Netdata](https://www.netdata.cloud/) - Troubleshoot slowdowns and anomalies in your infrastructure with thousands of metrics, interactive visualizations, and insightful health alarms.
- [Transmission](https://transmissionbt.com/) - is a feature-packed torrent client offering almost every function a torrent user will need.
- [NZBGet](https://nzbget.net/) - is a usenet downloader, written in C++ and designed with performance in mind to achieve maximum download speed by using very little system resources.
- [NPM](https://nginxproxymanager.com/) - is a reverse proxy management system based on an Nginx server and provides users with a clean, efficient, and beautiful web interface for easier management.
- [Navidrome](https://www.navidrome.org/) - allows you to enjoy your music collection from anywhere, by making it available through a modern Web UI and through a wide range of third-party compatible mobile apps, for both iOS and Android devices.

## Requirements

- dedicated server or PC with plenty of storage
- [docker](https://docs.docker.com/install/linux/docker-ce/debian/) and [docker-compose](https://docs.docker.com/compose/install/#install-compose)
- (optional) personal domain with configurable sub-domains (eg. plex.example.com)

## Direct Configuration

Copy `env.sample` to `.env` and populate all fields.

To add a non-existent shell user:

```bash
sudo useradd -r -s /bin/false USERNAME
```

## Deployment

Pull and deploy containers with docker-compose.

```bash
make deploy
```


## Author

Dimitris Matsoukas <https://github.com/99dimitris>

[Buy me a beer](https://www.buymeacoffee.com/dmatsoukas)

## Acknowledgments

I didn't create any of these docker images myself, so credit goes to the
maintainers, and the original software creators.

- <https://hub.docker.com/r/linuxserver/plex/>
- <https://hub.docker.com/r/linuxserver/jellyfin>
- <https://hub.docker.com/r/linuxserver/sonarr/>
- <https://hub.docker.com/r/linuxserver/radarr/>
- <https://hub.docker.com/r/linuxserver/bazarr>
- <https://hub.docker.com/r/linuxserver/lidarr>
- <https://hub.docker.com/r/linuxserver/prowlarr/>
- <https://hub.docker.com/r/linuxserver/nzbhydra2/>
- <https://hub.docker.com/r/linuxserver/ombi>
- <https://hub.docker.com/r/linuxserver/duplicati/>
- <https://hub.docker.com/r/netdata/netdata/>
- <https://hub.docker.com/r/linuxserver/transmission>
- <https://hub.docker.com/r/linuxserver/nzbget/>
- <https://hub.docker.com/r/jc21/nginx-proxy-manager>
- <https://hub.docker.com/r/deluan/navidrome>
