# General reuqirements

## Game roots

This peer-to-peer overlay network aims to be a simple and eays middleware for
creating scalable game networks. With the wish to support games comes a whole
range of other requirements. For example:

- low latency
- small network overhead
- small memory footprint
- interface potable to a lot of different languages (think Unity, Unreal engine,
  Godot, CryEngine and the like, each with it's own scripting capabilities)
- support for a wide range of architectures, OSs and devices

## Network roots

Being a peer-to-peer network comes with very own requirements. These are:

- serverless and self-organized operations.
- distributed ressources throughout all clients in the network

## Combined == peer-to-peer game

In addition, games and peer-to-peer networks combined add some more
requirements:

- trust management
- event notifications, including subscribing to, unsubscribing from, and 
  aggregations of eventstreams

## Resulting requirements

Consequently there are some things that can be decided for upfront to meet the
basic requirements on a very high level:

- Code comes in C++, because of native performance on a wide range of platforms

## Intended Users

This library is intended to be used for building games that expect its users to
be located around the globe and connected by the internet. General knowledge
about hardware architectures (x86, x86-64, ARM, PowerPC,...), networks (DNS,
Routing, OSI network layers, packets, UDP, ...) and operating systems (Windows,
Linux, MacOS, Android, iOS,...) is expected. Users should be intimately familiar
with their C++ compiler and C++11.

## Target platforms

This library is intended to be used primarily on x86-64 and ARM platforms.
Initial implementation will assume Linux as OS and will expand from there to
Windows, Android and iOS (possibly in that order).order

There will be no visual components, so porting to Smartphones, tablets, desktop
computers and other devices (internet of things, cloud computers SaaS providers)
shouldn't be a big issue.issue

## Detailed requirements

Please refer to the other documents in docs/requirements of this repository to
get detailed information about the requirements in this project