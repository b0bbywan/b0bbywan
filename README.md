> Senior R&D Engineer from Lille, France. 15 years in tech startups (gaming, SaaS, IoT, robotics, logistics). My background is in systems and infrastructure. DevOps culture shaped the way I write code: what I ship is built to run in production, deploy cleanly, and last.

## Stack

  <p align="center">
  <a href="https://go.dev/"><img src="https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white" alt="Go" /></a>
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white" alt="Python" /></a>
  <a href="https://www.kernel.org/"><img src="https://img.shields.io/badge/Linux-000000?logo=linux&logoColor=white" alt="Linux" /></a>
  <a href="https://www.gnu.org/software/bash/"><img src="https://img.shields.io/badge/Bash-4EAA25?logo=gnubash&logoColor=white" alt="Bash" /></a>
  <a href="https://www.ansible.com/"><img src="https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white" alt="Ansible" /></a>
  <a href="https://www.docker.com/"><img src="https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white" alt="Docker" /></a>
  <a href="https://www.postgresql.org/"><img src="https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white" alt="PostgreSQL" /></a>
  <a href="https://prometheus.io/"><img src="https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white" alt="Prometheus" /></a>
  <a href="https://grafana.com/"><img src="https://img.shields.io/badge/Grafana-F46800?logo=grafana&logoColor=white" alt="Grafana" /></a>
  <a href="https://aws.amazon.com/"><img src="https://img.shields.io/badge/AWS-232F3E?logo=amazonwebservices&logoColor=white" alt="AWS" /></a>
  <a href="https://github.com/features/actions"><img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white" alt="GitHub Actions" /></a>
  <a href="https://www.debian.org/doc/manuals/maint-guide/"><img src="https://img.shields.io/badge/Debian%20packaging-A81D33?logo=debian&logoColor=white" alt="Debian packaging" /></a>
  <a href="https://claude.com/claude-code"><img src="https://img.shields.io/badge/Claude%20Code-D97757?logo=claude&logoColor=white" alt="Claude Code" /></a>
  </p>

  <p align="center"><sub><em>minor stack</em></sub></p>

  <p align="center">
  <a href="https://www.home-assistant.io/"><img src="https://img.shields.io/badge/Home%20Assistant-18BCF2?logo=homeassistant&logoColor=white" alt="Home Assistant" /></a>
  <a href="https://hacs.xyz/"><img src="https://img.shields.io/badge/HACS-41BDF5?logo=homeassistantcommunitystore&logoColor=white" alt="HACS" /></a>
  <a href="https://www.musicpd.org/"><img src="https://img.shields.io/badge/MPD-A92E37" alt="MPD" /></a>
  <a href="https://www.freedesktop.org/wiki/Software/PulseAudio/"><img src="https://img.shields.io/badge/PulseAudio-2E3436?logo=pulseaudio&logoColor=white" alt="PulseAudio" /></a>
  <a href="https://htmx.org/"><img src="https://img.shields.io/badge/htmx-3366CC?logo=htmx&logoColor=white" alt="htmx" /></a>
  <a href="https://tailwindcss.com/"><img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?logo=tailwindcss&logoColor=white" alt="Tailwind CSS" /></a>
  <a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white" alt="TypeScript" /></a>
  <a href="https://vitejs.dev/"><img src="https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=white" alt="Vite" /></a>
  <a href="https://vercel.com/"><img src="https://img.shields.io/badge/Vercel-000000?logo=vercel&logoColor=white" alt="Vercel" /></a>
  </p>

## What I'm working on

### [odio](https://beta.odio.love) — an open source audio streaming platform for Linux

Turns any machine (even a 2012 Raspberry Pi B) into a full multi-room streamer: Bluetooth, AirPlay, Spotify Connect, UPnP/DLNA, CD playback. **No cloud, no account, no subscription.**

*A personal setup maintained in production for 6 years, turned into a complete installable product in 3 months.*

<p align="center">
  <img src="https://odio.love/screenshots/embedded-ui.png" alt="odio embedded web UI — full dashboard" width="48%">
  <img src="https://odio.love/screenshots/pwa-instances.png" alt="odio PWA — multi-node management" width="48%">
</p>

### Why odio is different

- **Runs in your systemd user session. Not as root.** No exclusive audio locks, no sudo-minefield.
- **All sources share one PulseAudio mixer.** MPD, shairport-sync, Snapclient, Bluetooth — you don't select a source, you just play.
- **API-first.** The REST API *is* the product; the web UI is just one client. Drives Home Assistant, the PWA, your shell, whatever you wire up.
- **Source-agnostic via MPRIS + D-Bus.** New players integrate without custom code.
- **Your streamer isn't a precious appliance — it's a reproducible host.** One command installs or reinstalls it. Safe to poke at, safe to break.

More on the philosophy: [how it works](https://docs.odio.love/guides/how-it-works/)

### Repositories

| Repository | Stack | Description |
|---|---|---|
| [go-odio-api](https://github.com/b0bbywan/go-odio-api) | ![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white) | REST API — D-Bus, PulseAudio, Bluetooth, MPRIS, systemd, Zeroconf, SSE, embed HTMX/Tailwind, multi-arch CI/CD, Debian packaging |
| [odio-ha](https://github.com/b0bbywan/odio-ha) | ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) | Home Assistant integration — Zeroconf, async SSE, native HA entities for each odio-api feature, HACS |
| [odios](https://github.com/b0bbywan/odios) | ![Ansible](https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white) | odio Streamer — Raspberry images, playbooks, curl \| bash install, multi-arch CI/CD |
| [odio-pwa](https://github.com/b0bbywan/odio-pwa) | ![Svelte](https://img.shields.io/badge/Svelte-FF3E00?logo=svelte&logoColor=white) | [Progressive Web App](https://pwa.odio.love) — SSE real-time, iframe |
| [go-mpd-discplayer](https://github.com/b0bbywan/go-mpd-discplayer) | ![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white) | CGo daemon — udev, MPD, CD/USB autoplay, multi-arch, Debian packaging |
| [go-disc-cuer](https://github.com/b0bbywan/go-disc-cuer) | ![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white) | CGo Lib/CLI — CD metadata via GNUDB/MusicBrainz |
| [go-odio-notify](https://github.com/b0bbywan/go-odio-notify) | ![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white) | Notification library — PulseAudio, pure Go, embedded sounds |
| [odio-apt-repo](https://github.com/b0bbywan/odio-apt-repo) | ![Debian](https://img.shields.io/badge/Debian-A81D33?logo=debian&logoColor=white) | APT repository — GitHub Actions, reprepro, GPG, multi-arch |
| [odio.love](https://github.com/b0bbywan/odio.love) | ![Astro](https://img.shields.io/badge/Astro-BC52EE?logo=astro&logoColor=white) | [Landing page](https://odio.love) — Svelte + Tailwind |
| [odio-docs](https://github.com/b0bbywan/odio-docs) | ![Astro](https://img.shields.io/badge/Astro-BC52EE?logo=astro&logoColor=white) | [Documentation site](https://docs.odio.love) — Starlight |


  ## Activity                                                                                                                                                                                                       
                  
  Live numbers across all odio repos, pulled from [docs.odio.love/stats.json](https://docs.odio.love/community/activity/) since January 2026.  
  
  <p align="center">
  <a href="https://docs.odio.love/community/activity/"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fdocs.odio.love%2Fstats.json&query=%24.totals.pr.merged&label=PRs%20merged&color=5ab81e"
   alt="PRs merged" /></a>
  <a href="https://docs.odio.love/community/activity/"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fdocs.odio.love%2Fstats.json&query=%24.totals.commits&label=commits&color=3a7020" 
  alt="commits" /></a>
  <a href="https://docs.odio.love/community/activity/"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fdocs.odio.love%2Fstats.json&query=%24.totals.releases&label=releases&color=BC52EE" 
  alt="releases" /></a>
  <a href="https://docs.odio.love/community/activity/"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fdocs.odio.love%2Fstats.json&query=%24.totals.stars&label=stars&color=F5C518" 
  alt="stars" /></a>
  <a href="https://docs.odio.love/community/activity/"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fdocs.odio.love%2Fstats.json&query=%24.totals.forks&label=forks&color=0082FC" 
  alt="forks" /></a>
  </p>  


## Elsewhere
  <p align="center">
  <a href="https://discord.gg/U9PyJMGg"><img src="https://img.shields.io/badge/Discord-5865F2?logo=discord&logoColor=white" alt="odio Discord" /></a>
  <a href="https://malt.fr/profile/mathieurequillart1"><img src="https://img.shields.io/badge/Malt-FC5757" alt="Malt freelance profile" /></a>
  <a href="https://medium.com/@mrequillart"><img src="https://img.shields.io/badge/Medium-000000?logo=medium&logoColor=white" alt="Medium" /></a>
  <a href="https://odio.love"><img src="https://img.shields.io/badge/odio.love-5ab81e" alt="odio.love project showcase" /></a>
  <a href="https://github.com/sponsors/b0bbywan"><img src="https://img.shields.io/github/sponsors/b0bbywan?label=Sponsor&logo=GitHub" alt="GitHub Sponsors" /></a>
  </p> 
