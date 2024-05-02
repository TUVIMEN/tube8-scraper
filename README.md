# tube8-scraper

A bash script for archiving tube8 videos, channels and pornstars metadata in json.

## Requirements

 - [reliq](https://github.com/TUVIMEN/reliq)
 - [jq](https://github.com/stedolan/jq)

## Installation

    install -m 755 tube8-scraper /usr/bin

## Json format

Here's example of a [video](video-example.json), [channel](channel-example.json) and [pornstar](pornstar-example.json).

## Usage

Results will be saved in files named by their sha256 hash of urls and placed in DIR.

Download metadata of videos in DIR using 8 threads

    tube8-scraper -t 8 -v DIR

Download metadata of pornstars in DIR

    tube8-scraper -p DIR

Download metadata of channels in DIR

    tube8-scraper -c DIR
