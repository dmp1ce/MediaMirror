# Media Mirror

Decentralized archive and media portal

## Description

The purpose of Media Mirror is to archive and index resources using a decentralized storage backends. Media Mirror targets [resources](Resource) and uses [fetcher](Fetcher) to retrieve the resource data. Media Mirror then can [version](Version) the resource data and store the version data in a [version storage](version storage).

### Resource

Resources are addresses or references to a media source. Examples could include `http` URL or IMDB ID.

### Fetcher

Fetchers are applications or methods used to download the resource data. A fetcher will create both a Examples could include `wget` or `youtube-dl` for a `http` resource. `dvdbackup` could be a fetcher for an IMDB ID.

### Version

A fetcher will create a version of a resource. Each user can independently verify or ignore a version in their archive. Versions are linked to the [resource](Resource) and [fetcher](Fetcher) used to create the version. Versions can have multiple [version storage](version storage) instances.

### Version Storage

Version storage is a reference to the version data. A version storage is linked to one [version](Version). A version storage example could be a torrent hash or magnet link or an IPFS URL.

## Roadmap

Currently, Media Mirror is only in the design and experimental phase. The plan is for Media Mirror to offer tools to create a peer-to-peer network for sharing media archive data. In addition, Media Mirror will provide tools to managing archives such as viewing, verifying and storing archives. Other tools will allow nodes to trust or block other peers on the network.
