<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/opendiscovery-logo-dark.svg">
    <img src="assets/opendiscovery-logo-light.svg" width="88" height="88" alt="OpenDiscovery">
  </picture>
</p>
<h1 align="center">OpenDiscovery</h1>
<p align="center">An agent workspace by General Epistemics.</p>
<p align="center"><a href="https://github.com/generalepistemics/opendiscovery-releases/releases">Downloads</a> · <a href="https://www.npmjs.com/package/@epistemics/opendiscovery-web">npm</a> · <a href="mailto:contact@kznlabz.com">Support</a></p>

Work with models, tools and project files through one web and desktop workspace. OpenDiscovery includes its native engine and connects sessions, permissions and project context across chat, terminals, Git worktrees and remote workspaces.

## Work in one place

- Configure model providers, tools, permissions and extensions.
- Run parallel sessions, review changes and combine results with Fusion.
- Set goals and scheduled tasks that continue while the browser is closed.
- Browse project files, use terminals and manage Git worktrees.
- Connect remote projects through SSH or container workspaces.

Models require your own configured provider access. Optional hosted services require compatible configured infrastructure.

## Choose a distribution

Only assets attached to a published release are available downloads. Read that release's installation guide and platform requirements before installing.

| Distribution | Targets | Start here |
| --- | --- | --- |
| Desktop | Linux x64/ARM64; Windows x64/ARM64 | Choose the installer for your operating system and architecture |
| Web/server | Linux glibc and Windows, x64/ARM64 | Install the npm package with Node 24.14.0 or newer |
| Docker | Linux x64 | Load the image archive and mount persistent data and your projects |
| Nix | `x86_64-linux` | Import the runtime closure using its included installation metadata |

Windows installers are unsigned. macOS, mobile and editor packages are not currently distributed.

### Web/server preview

```sh
npm install --global @epistemics/opendiscovery-web@alpha
opendiscovery serve --foreground --host 127.0.0.1 --port 3000
```

Keep npm optional dependencies enabled: they supply the matching native runtime. Open [localhost:3000](http://127.0.0.1:3000), select your project, connect a provider in **Settings → Providers**, then choose a model.

## Documentation and updates

Each release includes an offline documentation archive. Extract it and open `index.html` for installation, provider setup, permissions, remote access, extensions and troubleshooting.

```text
Release
├── Desktop installers
├── Web/server and npm runtime packages
├── Docker image and Nix runtime archives
├── Offline documentation
├── Update feeds
└── Release manifest, checksums and legal notices
```

Application and engine update together. Desktop uses the release's update feed; npm users run `opendiscovery update`. Follow the documentation for Docker and Nix updates. Check the release manifest and checksums when downloading archives.

The source repository is maintained privately. This repository hosts official downloads and user-facing release material.

## Support

Contact [contact@kznlabz.com](mailto:contact@kznlabz.com) for support or private security reports. Include your product version, operating system and distribution. Remove credentials and personal project data from logs before sharing.

OpenDiscovery includes third-party software. Applicable licenses and attribution are provided in [LICENSE.txt](LICENSE.txt), [NOTICE.txt](NOTICE.txt) and the distributed packages.
