
# Awesome maloja
[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

A list of software and services related to the open source self-hosted scrobble server [maloja](https://github.com/krateng/maloja).

Join the [maloja Unofficial Community Discord Server](https://discord.gg/TqkuVdnYPC) for assistance with maloja, and a welcoming community.

## Client Libraries

[mljcl](https://github.com/duckfromdiscord/mljcl) - My own maloja client library, written in Rust. It allows scrobbling, fetching of scrobble history, ranks, etc.

## Containers

[Docker](https://www.docker.com/) - An easy-to-use container platform. Also allows you to expose one folder to maloja's container that will contain all of its data. maloja comes with a Containerfile and [instructions](https://github.com/krateng/maloja?tab=readme-ov-file#docker--podman) on how to use it with Docker 

[podman](https://podman.io/get-started) - A more secure alternative to Docker that is compatible with existing Containerfiles. maloja is compatible with Docker and you can use the same image.

## Compatibility
This section describes ways to modify existing programs to work with maloja by redirecting already working scrobble clients to its recreated API endpoints like Audioscrobbler and Listenbrainz.

[Logitech Media Server plugin](https://forums.slimdevices.com/forum/user-forums/3rd-party-software/109857-maloja-scobbler-support-with-modified-audioscrobbler-plugin) - A modification you can make to Logitech Media Server to scrobble to maloja's Audioscrobbler API endpoint.

## Frontends and Vizualizers

[mljboard](https://github.com/mljboard/mljboard) - My maloja discord bot. WIP. You can link your maloja server to this bot through commands and you can show off the scrobble count for your favorite artists, albums, and tracks. 

[mljtui](https://github.com/duckfromdiscord/mljtui) - My maloja TUI (Terminal User Interface). Displays scrobble history in the terminal, as well as album art using colored ASCII art.

## Scrobble Clients (w/ Native Support)

[as-scrobbler](https://github.com/duckfromdiscord/as-scrobbler) - My own scrobble client for the game Audiosurf. You install it into the game's DLL folder and it intercepts Audiosurf's Last.FM requests to then redirect them to maloja's native scrobble endpoint using mljcl.

[foo_maloja](https://github.com/ICTman1076/foo_maloja) -  A native maloja scrobbling plugin for the music player Foobar2000. Seems to only work with maloja servers running on ports 80 and 443.

[mpdscrobble](https://github.com/dbeley/mpdscrobble) - A scrobbler for MPD with native maloja support.

[multi-scrobbler](https://github.com/FoxxMD/multi-scrobbler) -  A self-hosted scrobble client that can take play data from multiple streaming services, and also Last.FM itself, and forwards to plenty of scrobble servers. Natively supports maloja! It is also one of the only scrobblers out there that will include a scrobble length when sending scrobbles to maloja. Allows scrobbling from Spotify, Deezer, MPRIS, and more.

[OngakuKiroku](https://github.com/Atelier-Shiori/OngakuKiroku) - A scrobbler for MacOS designed for Swinsian and iTunes. Native maloja scrobbling support.

[Pano Scrobbler](https://github.com/kawaiiDango/pano-scrobbler) - An Android scrobbler with native maloja support.

[Web Scrobbler](https://github.com/web-scrobbler/web-scrobbler) - A wonderful extension for just about every browser, Web Scrobbler allows you to scrobble from (almost) every music streaming website out there, and if you find one that isn't supported, you can make a pull request to fix that. It has native maloja support.
