# IPFS Podcasting

[IPFS](https://ipfs.io/) peer-to-peer hypermedia protocol designed to preserve and grow humanity's knowledge. Basically, it's kind of like Napster but for everything.

[IPFS Podcasting](https://ipfspodcasting.net/) use the IPFS technology allowing people to host their own(or anyones) podcast episodes. No longer do you have the rely on Podcast providers.

IPFS Podcasting backs up your favorite shows and allows you to share them directly with people.

## Linux

### Pre-Installed IPFS

If you already have an IPFS server, you only need to run a client script every 10 minutes (via cron) to request & process podcast episodes.

1. [Download the client script](https://raw.githubusercontent.com/Cameron-IPFSPodcasting/podcastnode-Python/main/ipfspodcastnode.py).

2. Create a cron task to run the script every 10 minutes using flock to prevent multiple instances. You may optionally include your email address in the cron task to [manage your node](https://ipfspodcasting.net/Manage) from the website.

```*/10 * * * * cd ~/ && /usr/bin/flock -n /tmp/ipfspodcastnode.lockfile ~/ipfspodcastnode.py email@example.com```

### Install Script

If you don't have IPFS installed, this Install Script will install the latest IPFS software, IPFS Podcasting client script, and setup a cron task on your [Debian](https://www.debian.org/) or [Ubuntu](https://ubuntu.com/download) based PC (preferred).

1. [Download the install script](https://raw.githubusercontent.com/Cameron-IPFSPodcasting/podcastnode-Python/main/ipfspodcasting-install.sh).

2. Run the script with ```sudo bash ipfspodcasting-install.sh```

### Post Install

An ```ipfspodcastnode.log``` log file will be created to monitor activity.

If you've configured your email, you can [create an account](https://ipfspodcasting.net/Manage) to [manage your node](https://ipfspodcasting.net/Manage) and ["Favorite" feeds](https://ipfspodcasting.net/Help/Favorites) to support a podcast feed with long term hosting.

You can [view participating nodes](https://ipfspodcasting.net/PodSwarm) to find your node stats (using your IPFS ID).

### Troubleshooting & Support

For support, you can email <support@ipfspodcasting.net>, submit an issue at the [GitHub page](https://github.com/Cameron-IPFSPodcasting/podcastnode-Python/issues), or ask for help to [@Cameron](https://podcastindex.social/@cameron) on Mastodon [@podcastindex.social](https://podcastindex.social/).

## Mac

## Windows

## Umbrel OS
There is also an [IPFS Podcasting App](https://github.com/Cameron-IPFSPodcasting/podcastnode-Umbrel) for Umbrel OS.

1. Visit <https://umbrel.com/#start> for instructions installing Umbrel OS on a Raspberry PI or any [Debian](https://www.debian.org/) or [Ubuntu](https://ubuntu.com/download) based PC.

2. Install the IPFS Podcasting app from the Umbrel App store.

Optionally enter your email inside the app to [manage your node](https://ipfspodcasting.net/Manage) and ["Favorite" feeds](https://ipfspodcasting.net/Help/Favorites) from the website.

![image](https://user-images.githubusercontent.com/103131615/181662468-40d28845-aec7-48ce-9297-ccc4c788bfd2.png)

## Links
