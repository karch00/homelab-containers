# Server dockerfiles
Here I will upload and backup/make a sample the docker images for most of the services running on my homelab.<br>
Sensible/Variable information is redacted and require a `.env` file to replace the variables.

All (Most) services are *expected* to run behind a proxy regardless of if the service includes its own.<br>
Could be **nginx** or **caddy**, as preferred. Some services require websocket support.<br>

> [!WARNING]
> Some of the services may require extra config or differ building method.
> e.g. Extra config files, extra .env files, build from repo

## Service Containers

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/crafty-controller.svg" height="40" align="center" /> **[ [Crafty](https://gitlab.com/crafty-controller/crafty-4) ]**
Crafty is a **minecraft server hosting** service that lets users create and run servers alongside a 
*very* useful dashboard, allowing for multiple administrators to access the server's root directory
and run commands on the terminal (among other utilities).

Most of the time off, turn on only when friends of mine and I have a deep yearning for playing
together.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/excalidraw.svg" height="40" align="center" /> **[ [Excalidraw](https://github.com/excalidraw/excalidraw) ]**
Excalidraw is a user-friendly **workflow designing** web app. It lets the user create a simple *yet*
effective workflow using shapes, text, arrow relations, etc.<br>
Each element is very customizable: line art, font, background of each element...<br>
Has its own **[website](https://excalidraw.com/)** that can be used for free with *some* features
that require their **excalidraw+** subscription.

Self-host it to add these premium features for free.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/forgejo.svg" height="40" align="center" /> **[ [Forgejo](https://codeberg.org/forgejo/forgejo) ]**
Forgejo is a **git server** that serves to host your own repositories just as **github**, **codeberg**
or **gitlab** would let you, but self-hosted.<br>
It has some limitations compared to the aforementioned, but it is still an extremely powerful 
tool for having your own centralised repositories.

Mostly use it to host quick backups/versioning of more personal work that would be better off the
public access.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/freshrss.svg" height="40" align="center" /> **[ [Freshrss](https://github.com/FreshRSS/FreshRSS) ]**
Freshrss is a **custom RSS feed** that lets the user customize their own feed from various RSS sources.<br>
It is very customizable and respects the requested RSS page's limitations. Interface is very pleasant
and reader-friendly and allows for quick debugging of why a feed might not be compatible, stopped working,
etc.

**Very** useful service for my custom news feed. Have many categories set up with various feeds attached to
each.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/headscale.svg" width="40" align="center" /> **[ [Headscale](https://github.com/juanfont/headscale) ]**
Headscale is a **tailscale-compatible server** which serves as a custom VPN/mesh network.<br>
Very easy to set up and get running and since it is tailscale-compatible, connecting to it is a breeze.
It is extremely customizable via de settings for a better experience.

Use it to tunnel my connection from *anywhere* outside my home serving as an encrypted proxy.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/png/homepage.png" height="40" align="center" /> **[ [Homepage](https://github.com/gethomepage/homepage) ]**
Homepage is an extremely customizable **dashboard** let ting you create your own homepage
with widgets, service statuses and bookmarks.<br>
Style and behaviour is customizable via `custom.css` and `custom.js`. Custom assets can be added and
used with ease.

Use it for my homelab's homepage/dashboard behind an **authentification layer** to restrict unwanted
access/info scrapping.

### <img src="https://cdn.jsdelivr.net/gh/selfhst/icons/svg/it-tools.svg" height="40" align="center" /> **[ [ItTools](https://github.com/CorentinTh/it-tools) ]**
ItTools is a **consortium of IT-related tools**. It has almost anything you might need: Base conversion,
Hash generation, Token generation, password strength test...

Very versatile and useful, use it from time to time for general tasks I would rather have it done quick than
use the CLI or rely an external service.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/jellyfin.svg" height="40" align="center" /> **[ [Jellyfinn](https://github.com/jellyfin/jellyfin) ]**
Jellyfinn is a popular **personal video streaming** platform that lets the user host their own libraries 
with their *own*series, anime or movies. It features automatic metadata collection via IMDd and a quite 
complete user managementfor your family, your friend group, etc.

Use it for my own personal series and movies. Comes in very handy when you own a series/movie that is not available
in your go-to subscription site, or at all really.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/kavita.svg" height="40" align="center" /> **[ [Kavita](https://github.com/Kareadita/Kavita) ]**
Kavita is a **personal book hosting** platform, similar to jellyfinn it lets the user hot their own book
libraries and personalize users. It supports a variety of book formats such as Epub or PDF and even image formats.

Same as jellyfinn, use it to host my *owned* books for personal reading.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/myspeed.svg" height="40" align="center" /> **[ [MySpeed](https://github.com/gnmyt/myspeed) ]**
MySpeed is a simple **speed test** application which tests the speed and bandwidth of your server towards 
the exterior of your network via a connexion to third party testing websites.

Set to periodically run a test to show the results on my dashboard.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/n8n.svg" width="40" align="center" /> **[ [n8n](https://github.com/n8n-io/n8n) ]**
n8n is a **workflow automation** service that serves to automate any kind of workflow with an easy-to-read interface
and a many out-of-the-box functionality.<br>
It allows for any automation from a simple `trigger -> action` to an entire complex workflow with conditions and
edge cases.

Mostly use it for some simple automation regarding my homelab's health.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/png/navidrome.png" height="40" align="center" />**[ [Navidrome](https://github.com/navidrome/navidrome) ]**
Navidrome is a **personal music streaming** platform that lets the user host their own music files. Its UI is
very versatile and intuitive and supports multiple users and shared playlists.

Use it for my own personal streaming, anywhere anytime.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/nextcloud.svg" width="40" align="center" />**[ [Nextcloud](https://github.com/nextcloud) ]**
Nextcloud is a complete **cloud file drive** platform with a very friendly UI and extensive platform compatibility.
It supports many users with their own drives, quotas, sharing, and collaborative document editing.

Use it very frequently for file backup, storage and giving some friends some free cloud storage.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/stirling-pdf.svg" height="40" align="center" /> **[ [StirlingPDF](https://github.com/Stirling-Tools/Stirling-PDF) ]**
StirlingPDF is a complete **PDF manipulation** tool with a friendly UI and powerful functionalities.<br>
Although for single users it is completely free, having more than 3 individual users logged requires a paid subsription.
This makes it powerful for individual users that are sceptical their data might be stored on third party websites
(rightfully so).

As described before, I use it to manipulate PDFs without having to rely on third-party services. Me being an individual,
the subscription con does not concern me so much.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/stoat.svg" height="40" align="center" /> **[ [Stoat](https://github.com/stoatchat/stoatchat) ]**
Stoat is a **discord-like communication** platform that supports an extreme level of customization and compatible with
most platforms, accessible via web. Support for text, automatic link embeds, voice calls, video calls and screensharing<br>
This runs as your own discord instance, where multiple users, groups and servers can be found. It offers both the host user
and the end user an extreme level of customization, functionality-wise and appearance-wise. <br>

Mostly an experiment to see how I could integrate and interact with my friends in the case discord/institutions adopt a more
extreme stance that would jeopardize privacy.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/tinyauth.svg" height="40" align="center" /> **[ [TinyAuth](https://github.com/tinyauthapp/tinyauth) ]**
TinyAuth is a **lightweight authentication** service that allows users to add an authentication layer to their services/pages.

Used to add an authentication layer in front of my authentication-less services, primarily my dashboard for now.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/uptime-kuma.svg" height="40" align="center" /> **[ [UptimeKuma](https://github.com/louislam/uptime-kuma) ]**
UptimeKuma is a lightweight yet complete **uptime monitoring** service.<br>
Allows user to monitor the uptime of any website/service with configurable settings for intervals, retries, timeout, TLS, etc.

Have it running pointing at my main services for insight via my dashboard.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/vaultwarden.svg" height="40" align="center" /> **[ [VaultWarden](https://github.com/dani-garcia/vaultwarden) ]**
VaultWarden is a **BitWarden-compatible server** that allows users to store personal login informations per-page and create
organizations for a hierarchical order with authority levels.

Strictly for personal use running for all my devices to sync to the bitwarden extension.

### <img src="https://cdn.jsdelivr.net/gh/homarr-labs/dashboard-icons/svg/wger.svg" height="40" align="center" /> **[ [Wger](https://github.com/wger-project/wger) ]**
Wgerr is a very complete **Fitness tracker** that lets the end user create, edit, organize and track their fitness goals:
Diets, Routines, Measurements, etc.<br>
It is very user-friendly and supports both web and application access.

Use it *daily* to track all my fitness-related goals.
