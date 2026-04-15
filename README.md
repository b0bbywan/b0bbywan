> Senior R&D Engineer from Lille, France. 15 years in tech startups (gaming, SaaS, IoT, robotics, logistics). My background is in systems and infrastructure. DevOps culture shaped the way I write code: what I ship is built to run in production, deploy cleanly, and last.

## What I'm working on

**[odio](https://beta.odio.love)** — An open source audio streaming platform for Linux. Turns any machine (even a 2012 Raspberry Pi B) into a full multi-room streamer: Bluetooth, AirPlay, Spotify Connect, UPnP/DLNA, CD playback. No cloud, no account, no subscription.

A personal setup maintained in production for 6 years, turned into a complete installable product in 3 months.

| Repository | Description |
|---|---|
| [go-odio-api](https://github.com/b0bbywan/go-odio-api) | Go REST API — D-Bus, PulseAudio, Bluetooth, MPRIS, systemd, Zeroconf, SSE, embed HTMX/Tailwind, multi-arch CI/CD, Debian packaging |
| [odio-ha](https://github.com/b0bbywan/odio-ha) | Home Assistant integration — Zeroconf, async SSE, native HA entities for each odio-api feature, HACS |
| [odios](https://github.com/b0bbywan/odios) | odio Streamer — Raspberry images, Ansible playbooks, curl | bash install, multi-arch CI/CD |
| [odio-pwa](https://github.com/b0bbywan/odio-pwa) | [Progressive Web App](https://pwa.odio.love) — Svelte 5, SSE real-time, iframe |
| [go-mpd-discplayer](https://github.com/b0bbywan/go-mpd-discplayer) | Go + CGo daemon — udev, MPD, CD/USB autoplay, multi-arch, Debian packaging |
| [go-cd-cuer](https://github.com/b0bbywan/go-cd-cuer) | Go + CGo Lib/CLI — CD metadata via GNUDB/MusicBrainz |
| [go-odio-notify](https://github.com/b0bbywan/go-odio-notify) | Go notification library — PulseAudio, pure Go, embedded sounds |
| [odio-apt-repo](https://github.com/b0bbywan/odio-apt-repo) | Debian APT repository — GitHub Actions, reprepro, GPG, multi-arch |
| [odio.love](https://github.com/b0bbywan/odio.love) | [Landing page](https://odio.love) — Astro + Svelte + Tailwind |
| [odio-docs](https://github.com/b0bbywan/odio-docs) | [Documentation site](https://docs.odio.love) — Starlight, Astro |

## Stack

Go · Python · Linux · Ansible · Docker · PostgreSQL · Prometheus · Grafana · GitHub Actions · Debian packaging

## Elsewhere

- [Malt](https://malt.fr/profile/mathieurequillart1) — Freelance profile
- [odio.love](https://beta.odio.love) — Project showcase
- [Medium](https://medium.com/@mrequillart) — multi-part series on Linux audio with Raspberry Pi
- [Sponsor me](https://github.com/sponsors/b0bbywan) — Help keep odio free and independent
