# Nova Player Kids

Personal NOVA Video Player fork designed to run alongside the regular NOVA app as a separate, kid-focused media player.

It keeps normal NOVA behaviour while using its own Android package, media-library namespace, and branding, allowing both apps to be installed on the same device with separate libraries.

## Features

- installs alongside regular NOVA Video Player
- separate app data and media library
- intended for kid-specific movie and TV libraries
- pink `KIDS` launcher icon and TV branding
- normal NOVA playback, scraping, library, and network features retained
- universal APK for Android TV and other supported Android devices

There is deliberately **no parental-control or content-filtering layer** in this fork.

**However**, what it *does* let you do is have TWO instances of NOVA Player simultaneously on your device, with each pointing to different directories. Eg:

Nova Player
- C:\movies
- C:\tv_shows

NovaPlayer Kids
- C:\Kids_movies
- C:\Kids_tv_shows 

Thus, you can hide one version of Nova Player behind a password as needed. 

The separation comes from running a second NOVA instance and pointing it only at the media sources you want available to kids.

## Current Build

The current build is **Nova Player Kids 6.4.64**, based on NOVA Video Player 6.4.64.

Side-by-side installation with regular NOVA has been tested successfully on Android and Google Chromecast with TV /Google TV devices.

Basic library population, launch, and playback have also been tested successfully.

Package:

`com.bobbyllm.novaplayerkids`

## Download

Download the current universal APK from [GitHub Releases](https://github.com/BobbyLLM/NovaPlayerKids/releases).

The universal APK includes support for the Android architectures provided by the upstream NOVA build.

## Repository Notes

This repository is maintained for *private* use, but you are WELCOME to use it :) 

I designed this because I really love NovaPlayer...but I don't want my kids looking at Tarantino films, Tru Blood, Alien etc. 

Unfortunately, at present, upstream Nova Player does not support parental controls, age-based filtering or multiple TV and Movie directories being displayed neatly. So, please accept this as a work around until such time as the wonderful team upstream figures out a better solution.  

Nova Player Kids intentionally stays very close to upstream NOVA. Changes are limited primarily to the separate application identity, provider namespace, and Kids branding required for side-by-side installation. TL;DR - if it's pink with KIDS on it (as my kids requested), it's the kids one :) 

The build is pinned to NOVA Video Player 6.4.64 rather than following moving upstream branches. Updates are unlikely unless I detect something that breaks locally. WYSIWYG.

Pull requests are *not* accepted. Sorry! Fork your own and go cook:)

*No* support or compatibility guarantee is provided.

## Based on NOVA Video Player

Nova Player Kids is a minimal fork of the excellent open-source [NOVA Video Player](https://github.com/nova-video-player/aos-AVP).

NOVA Video Player is licensed under the Apache License 2.0.

Upstream project:

https://github.com/nova-video-player/aos-AVP