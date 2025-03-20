> [!WARNING]
> Do not abuse this otherwise Github will disable your account.

### ℹ️ About
This creates temporary & ephemeral dev instances with SSH Access meant for testing builds & stuff.<br>

### 🖳 Config
- [Reusable TailScale Auth Key](https://login.tailscale.com/admin/settings/keys) as an Action Secrets: `TS_KEY` (Permissions: Pre-Approved, Ephemeral)
- [BlackSmith](https://docs.blacksmith.sh/introduction/quickstart) Configured on this Repository
- [SSH Public Keys](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) Configured on your Account `https://github.com/USERNAME.keys`

### 🧰 Container
- [Ubuntu-Systemd](https://github.com/pkgforge/devscripts/pkgs/container/devscripts%2Fubuntu-systemd-base): https://github.com/pkgforge/devscripts/blob/main/Github/Runners/ubuntu-systemd-base.dockerfile

### 🤖 Runners
- `gh-runner-aarch64`: Default Github's Ubuntu aarch64 Runner --> https://docs.github.com/en/actions/using-github-hosted-runners/using-github-hosted-runners/about-github-hosted-runners
- `gh-runner-x64`: Default Github's Ubuntu x86_64 Runner --> https://docs.github.com/en/actions/using-github-hosted-runners/using-github-hosted-runners/about-github-hosted-runners
- `bs-runner-aarch64`: Default Blacksmith's Ubuntu aarch64 Runner --> https://docs.blacksmith.sh/github-actions-runners/config#arm-runners
- `bs-runner-x64`: Default Blacksmith's Ubuntu x86_64 Runner --> https://docs.blacksmith.sh/github-actions-runners/config#x64-runners
