---
title: "Projects"
description: "Open source projects by Mike Oertli: developer tools, Kubernetes utilities, Raycast extensions, and shell scripting helpers."
showDate: false
showReadingTime: false
showPagination: false
showTableOfContents: true
---

A selection of my open source projects, from command-line tools to everyday workflow helpers. These are also featured in the pinned repositories on [my GitHub profile](https://github.com/mikeoertli), where you can explore more of my work.

These projects are a mix of hand-coded work, aggregation of concepts I like from other projects, and AI-assisted coding. The icons in particular are ultimately AI-generated. I am NOT a designer, nor could I dream of becoming one, so I find this to be the most reasonable way to get an icon for projects that do not warrant commissioning one.

Please provide feedback or PRs if you have ideas!

---

## 💻 Go TUIs

<div class="project-heading">

<a href="https://github.com/mikeoertli/github-pr-monitor"><img src="https://raw.githubusercontent.com/mikeoertli/github-pr-monitor/HEAD/assets/gprm-icon.png" alt="GitHub PR Monitor icon" width="64" loading="lazy" decoding="async"></a>

### GitHub PR Monitor

</div>

A terminal interface for keeping an eye on GitHub pull requests and their associated CI builds. It lets you view by Jira (or other tracking) ticket IDs if configured and makes it easy to navigate to the Jira ticket, GitHub PR page, CI build page, or to copy the `gh` CLI command to see status or the `curl` command to retrieve CI status.

**Language:** Go · [View on GitHub](https://github.com/mikeoertli/github-pr-monitor)

<a href="https://raw.githubusercontent.com/mikeoertli/github-pr-monitor/HEAD/assets/gprm-demo.gif"><img src="https://raw.githubusercontent.com/mikeoertli/github-pr-monitor/HEAD/assets/gprm-demo.gif" alt="GitHub PR Monitor demo showing pull requests and CI build progress" loading="lazy" decoding="async" style="width: 100%; height: auto;"></a>

<div class="project-heading">

<a href="https://github.com/mikeoertli/kube-resource-monitor"><img src="https://raw.githubusercontent.com/mikeoertli/kube-resource-monitor/HEAD/assets/png/icon-128.png" alt="Kubernetes Resource Monitor icon" width="64" loading="lazy" decoding="async"></a>

### Kubernetes Resource Monitor

</div>

I have been severly underwhelmed by other Kubernetes resource monitoring solutions. I feel like I have tried them all, and it is annoying to have to use a browser or GUI application all the time to simply see how things look in a cluster.

This is my solution to a terminal interface for monitoring Kubernetes resources.

**Language:** Go · [View on GitHub](https://github.com/mikeoertli/kube-resource-monitor)

<a href="https://raw.githubusercontent.com/mikeoertli/kube-resource-monitor/HEAD/assets/krm-demo.gif"><img src="https://raw.githubusercontent.com/mikeoertli/kube-resource-monitor/HEAD/assets/krm-demo.gif" alt="Kubernetes Resource Monitor demo showing resource usage and workload details" loading="lazy" decoding="async" style="width: 100%; height: auto;"></a>


<div class="project-heading">

<a href="https://github.com/mikeoertli/kube-context-manager"><img src="https://raw.githubusercontent.com/mikeoertli/kube-context-manager/HEAD/assets/icon.png" alt="Kubernetes Context Manager icon" width="64" loading="lazy" decoding="async"></a>

### Kubernetes Context Manager

</div>

A Kubernetes context manager inspired by `kubectx`. The key difference here is that it is based on supporting different "profiles" and a profile can have associated protections (like expiration) so that you don't leave a global kube context set for any/all shells by accident.

For example, local is the default, then `dev` is for shared clusters which are in flux and not sacrosanct, then you can have `perf` clusters which can be used but you want to be careful, and `prod` which has a short timeout (where the kube config resets to local on expiration).

**Language:** Go · [View on GitHub](https://github.com/mikeoertli/kube-context-manager)

<a href="https://raw.githubusercontent.com/mikeoertli/kube-context-manager/HEAD/assets/demo.gif"><img src="https://raw.githubusercontent.com/mikeoertli/kube-context-manager/HEAD/assets/demo.gif" alt="Kubernetes Context Manager demo showing profiles, contexts, namespaces, and expiration" loading="lazy" decoding="async" style="width: 100%; height: auto;"></a>

<div class="project-heading">

<a href="https://github.com/mikeoertli/shell-charm-progress"><img src="https://raw.githubusercontent.com/mikeoertli/shell-charm-progress/HEAD/assets/shell-charm-progress-icon.png" alt="Shell Charm Progress icon" width="64" loading="lazy" decoding="async"></a>

### Shell Charm Progress

</div>

I wanted a quick and easy way to use progress bars in my shell scripts. I didn't find a suitable solution for that, so I built it.

This is a standalone, Charm-styled progress bar that can be controlled from a shell script.

**Language:** Go · [View on GitHub](https://github.com/mikeoertli/shell-charm-progress)

<a href="https://raw.githubusercontent.com/mikeoertli/shell-charm-progress/HEAD/assets/shell-charm-progress-demo.gif"><img src="https://raw.githubusercontent.com/mikeoertli/shell-charm-progress/HEAD/assets/shell-charm-progress-demo.gif" alt="Shell Charm Progress demo showing simulated repository updates above a purple-to-pink progress bar" loading="lazy" decoding="async" style="width: 100%; height: auto;"></a>

---

## 🤓 Shell Scripts

I am a big fan of shell scripts, and every time I go to write one, I seem to learn new features and capabilities. 

My dotfiles are still private. They are extensive to say the least, but not yet in a state where I can share them. However, I deeply love tinkering with dotfiles, so if you ever have ideas or want to chat, please don't hesitate to reach out.

<div class="project-heading">

<a href="https://github.com/mikeoertli/shell-script-template"><img src="https://raw.githubusercontent.com/mikeoertli/shell-script-template/HEAD/assets/icon-512.png" alt="Shell Script Template icon" width="64" loading="lazy" decoding="async"></a>

### Shell Script Template (Bash)

</div>

I maintain this template as my starting point for new shell scripts. I mainly use macOS, but aim for compatibility with both its bundled Bash 3.2 and modern Bash 5.x releases, while avoiding macOS-specific dependencies.

**Language:** Bash · [View on GitHub](https://github.com/mikeoertli/shell-script-template)

<a href="https://raw.githubusercontent.com/mikeoertli/shell-script-template/HEAD/assets/progress-bar-demo.gif"><img src="https://raw.githubusercontent.com/mikeoertli/shell-script-template/HEAD/assets/progress-bar-demo.gif" alt="Shell Script Template progress bar example showing three simulated jobs with live output and completion counts" loading="lazy" decoding="async" style="width: 100%; height: auto;"></a>

---

## ✨ Raycast Extensions

<div class="project-heading">

<a href="https://github.com/mikeoertli/raycast_webpage_to_markdown"><img src="https://raw.githubusercontent.com/mikeoertli/raycast_webpage_to_markdown/HEAD/webpage-to-markdown-local/assets/webpage-to-markdown-logo.png" alt="Webpage to Markdown icon" width="64" loading="lazy" decoding="async"></a>

### Webpage to Markdown

</div>

A Raycast tool that converts webpages to Markdown. All conversion happens **locally**, keeping the conversion private without relying on cloud conversion services. It can also capture assets for a fully offline export.

**Language:** TypeScript · [View on GitHub](https://github.com/mikeoertli/raycast_webpage_to_markdown)


