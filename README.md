# ping-monitor
Ping Monitor APP for Linux
# Ping Monitor

A lightweight desktop ping monitor for Ubuntu. Add servers, see their status at a glance (green = up, red = down), and check round-trip latency — all checked automatically every 30 seconds via ICMP.

![Ping Monitor screenshot](https://github.com/polarispantoja/ping-monitor/blob/main/Screenshot%20from%202026-06-19%2010-20-42.png)

## Features

- **Add & remove servers** from a simple UI
- **Real-time status dots**: green (up) / red (down)
- **Latency display** in milliseconds
- **Automatic checks** every 30 seconds
- **Persistent server list** saved to `~/.config/PingMonitor/servers.json`
- Uses the system's built-in `ping` command — no root required

## Install

Download the latest release from the [Releases](https://github.com/polarispantoja/ping-monitor/releases) page, or build from source:

```bash
git clone https://github.com/polarispantoja/ping-monitor.git
cd ping-monitor/desktop-app
npm install
npm start
```

To package for distribution:

```bash
npm run package
```

This creates `release/PingMonitor-linux-x64/` which you can run directly or archive.

## Built With

- **[Electron](https://www.electronjs.org/)** — Cross-platform desktop app framework ([MIT License](https://github.com/electron/electron/blob/main/LICENSE))
- Built and scaffolded with **[Lovable](https://lovable.dev)** — AI-powered full-stack app builder

## Credits & Licenses

This project uses open-source software. The application logic and UI in this repository are original work, while the underlying runtime and build tooling carry their own licenses:

| Dependency | License | Source |
|------------|---------|--------|
| Electron | [MIT](https://github.com/electron/electron/blob/main/LICENSE) | https://github.com/electron/electron |
| electron-packager | [BSD-2-Clause](https://github.com/electron/packager/blob/main/LICENSE) | https://github.com/electron/packager |

## License

This project (the original application code in this repository) is released under the **MIT License**. See `LICENSE` for details.

> **Note:** Electron and its related packages are separately licensed by their respective authors. When distributing a packaged Electron app, you are also distributing Electron's runtime, which is licensed under the MIT License. No additional attribution is strictly required beyond retaining Electron's license file in the distribution, but linking to the project above is good practice.
