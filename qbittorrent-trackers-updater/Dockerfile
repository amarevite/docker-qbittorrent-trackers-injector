FROM alpine:latest

RUN apk add --no-cache bash curl jq

ADD https://raw.githubusercontent.com/GreatNewHope/jorman_scripts/refs/heads/master/AddqBittorrentTrackers/AddqBittorrentTrackers.sh /AddqBittorrentTrackers.sh

COPY qbittorrent-trackers-updater/entrypoint.sh /entrypoint.sh
RUN chmod +x /AddqBittorrentTrackers.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
