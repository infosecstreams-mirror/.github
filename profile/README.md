# Welcome to the InfoSec Streams Mirror (UK) 🇬🇧

[![Website](https://img.shields.io/badge/Website-infosecstreams.wupinyin.co.uk-blue?style=for-the-badge)](https://infosecstreams.wupinyin.co.uk)

We are a UK-based, community-maintained mirror of the popular InfoSec Streams project. Our goal is to provide a frictionless, accessible, and highly resilient directory of the best cybersecurity, hacking, and OSINT content creators across Twitch and YouTube.

---

## 🚀 Why we exist
This mirror was completely re-architected by **[Wupinyin](https://github.com/DiscoMouse)** to build a decentralized, "resilient network in code." We moved away from the fragile, statically generated cron-jobs of the original project and fully decoupled the frontend from the backend!

- ⚡ **Dynamic REST API**: We rebuilt the backend as a blazing-fast, containerized Golang REST API that instantly serves live streamer statuses from a PostgreSQL database, triggered by real-time Twitch Webhooks.
- 🎨 **Decoupled Template Frontend**: The frontend is now a pure UI layer that consumes the API. No more hardcoded tables or static generation!
- 🔒 **Self-Hosted Privacy**: We removed third-party analytics and external CDNs. All assets are self-hosted to respect privacy.

## 📌 Our Projects

* [**StreamStatus Backend**](https://github.com/infosecstreams-mirror/StreamStatus) - The high-performance Golang backend API and Twitch EventSub webhook handler.
* [**Frontend Template**](https://github.com/infosecstreams-mirror/infosecstreams.github.io) - The pure Jekyll-based static site template.
* [**Our Live UK Mirror**](https://github.com/infosecstreams-mirror/infosecstreams-mirror-uk-wupinyin) - The actual GitHub Pages deployment for `infosecstreams.wupinyin.co.uk`.

## 🌍 Create Your Own Mirror!

We want to build a resilient, globally distributed network of InfoSec Streams. You can deploy your own mirror in minutes:

1. **Host an API Node:** Grab our `StreamStatus` backend code and run it on your own server or container.
2. **Deploy the Frontend:** Go to our [Frontend Template](https://github.com/infosecstreams-mirror/infosecstreams.github.io) and click **"Use this template"** to instantly spin up your own customized UI on GitHub Pages.
3. **Connect them:** Simply edit `js/sort.js` in your new repository and change the `API_ENDPOINT` constant to point to your new API node!

You now have a fully functional, auto-updating directory of your own!

## 🤝 Getting Involved

Whether you want to add yourself to our UK directory or submit a patch to the codebase:
1. Check out our **Issues** tab to request addition to the streamers list (we are building an automated approval workflow soon!).
2. Feel free to open a ticket if you find a bug in the API or the UI.
