<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/obelisk-dark.png">
  <img src="assets/obelisk-light.png" alt="Obelisk" width="180">
</picture>

# Obelisk

**Private, local-first tools for running your own life.**

No account. No cloud. No telemetry. Your data is a file on your disk,
and you can read it without us.

<sub>
  local-first · no telemetry · open source · Linux
</sub>

</div>

---

## Install

The launcher is the only thing you install by hand. Everything else is
installed from inside it, and uninstalls through your system's own app list
whether or not the launcher is still around.

<details open>
<summary><b>Debian, Ubuntu, Mint</b></summary>

```bash
curl -L https://github.com/bogdan-tr/obelisk-suite/releases/latest/download/obelisk-shell_amd64.deb -o /tmp/obelisk.deb
sudo apt install /tmp/obelisk.deb
```

</details>

<details>
<summary><b>Fedora, RHEL, openSUSE</b></summary>

```bash
curl -L https://github.com/bogdan-tr/obelisk-suite/releases/latest/download/obelisk-shell_x86_64.rpm -o /tmp/obelisk.rpm
sudo dnf install /tmp/obelisk.rpm
```

</details>

<details>
<summary><b>Any Linux — no install, just run it</b></summary>

```bash
curl -L https://github.com/bogdan-tr/obelisk-suite/releases/latest/download/obelisk-shell_amd64.AppImage -o obelisk
chmod +x obelisk
./obelisk
```

</details>

<details>
<summary><b>Windows and macOS</b></summary>

Not built yet. The release pipeline supports both, but nothing has been
published for them, so there is no command here that would work.

</details>

> **Why there is no `curl … | sh` here.**
> The usual one-liner pipes a script straight into your shell. For a project
> whose entire claim is that it does not phone home, asking you to execute an
> unread remote script would be a poor first thing to ask. Every command above
> is one you can read in full before running it.

---

## The apps

<table>
<tr>
<td width="120" align="center" valign="middle">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/taskmancer-dark.png">
    <img src="assets/taskmancer-light.png" alt="" width="88">
  </picture>
</td>
<td valign="middle">

### Taskmancer

**Most task apps remember what you owe. This one tells you what it will
cost.**

- **A week you can see before you reach it.** Every day shows its predicted
  hours against your own target, so next Thursday has a weight before
  Thursday arrives.
- **Estimates that pay for themselves.** Rough is fine — the app shows you
  the gap between estimate and reality, and you get better at it.
- **Yours to shape.** Your own statuses, priorities, views and cards.
  Thirty-odd themes, sounds, and a layout you arrange.

<sub>Available now · Linux</sub>

</td>
</tr>
</table>

<details>
<summary><b>More about Taskmancer</b></summary>

<br>

*Screenshots go here.*

**Chains and subtasks.** A chain runs in order — finish one link and the next
opens itself. New links inherit the chain's own defaults, so you set things
once rather than every time.

**Recurrence that behaves.** Series generate real occurrences you can move,
pause for a fortnight, and resume without losing what you changed.

**Time tracking, and what it is for.** Tracked time feeds the forecast. That
is the whole point of it — not a report you never read, but the thing that
makes next week's number true.

**A day you can plan against real hours.** Lay today's work onto a timeline
and see whether it actually fits. What does not fit is the useful part.

**Keyboard first.** `Ctrl+T` anywhere for a new task, `Ctrl+F` to find,
`Ctrl+K` to jump. Vim motions where lists are.

</details>

---

## Coming

Each of these has a design, a spec and a name. None has a release yet, and
they are listed so you know where this is going — not as a promise about
when.

<table>
<tr>
<td width="64" align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/zoryndor-dark.png"><img src="assets/zoryndor-light.png" alt="" width="44"></picture></td>
<td><b>Zoryndor</b><br><sub>A calendar that is actually yours. Views, recurrence, drag to reschedule.</sub></td>
</tr>
<tr>
<td width="64" align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/dream-dark.png"><img src="assets/dream-light.png" alt="" width="44"></picture></td>
<td><b>Dream</b><br><sub>A dream journal with voice capture, auto-tagging, and analysis that runs on your own machine.</sub></td>
</tr>
<tr>
<td width="64" align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/kupal-dark.png"><img src="assets/kupal-light.png" alt="" width="44"></picture></td>
<td><b>Kupal</b><br><sub>Habits, without the streak guilt.</sub></td>
</tr>
<tr>
<td width="64" align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/photos-dark.png"><img src="assets/photos-light.png" alt="" width="44"></picture></td>
<td><b>Photos</b><br><sub>Your library, on your disk, searchable without uploading it to anyone.</sub></td>
</tr>
<tr>
<td width="64" align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/alchemist-dark.png"><img src="assets/alchemist-light.png" alt="" width="44"></picture></td>
<td><b>Alchemist</b><br><sub>Research notes that hold their shape as a project grows.</sub></td>
</tr>
<tr>
<td width="64" align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/obsidian-bridge-dark.png"><img src="assets/obsidian-bridge-light.png" alt="" width="44"></picture></td>
<td><b>Obsidian Bridge</b><br><sub>Two-way sync between the suite and an Obsidian vault.</sub></td>
</tr>
</table>

---

## What "local-first" means here

<details open>
<summary><b>The short version</b></summary>

<br>

- **No account.** There is nothing to sign up for.
- **No network at rest.** The apps talk to the internet to check for updates
  and to download one you asked for. That is all.
- **Your data is readable without us.** Tasks are files. Settings are JSON.
  If this project disappeared tomorrow you would still have everything, in
  formats you can open.
- **Updates are signed.** Each app verifies an update against a key compiled
  into it and refuses anything that does not check out, so a compromised
  release page cannot push you a replacement binary.

</details>

---

## Uninstalling

Through your system's normal app list — Add/Remove Programs, your
distribution's software centre, or `apt remove` / `dnf remove`. The launcher
hands packages to your OS installer rather than managing them itself, so
removing the launcher strands nothing.

Your data is deliberately left behind, so reinstalling picks up where you
left off. To remove it as well:

```bash
rm -rf ~/.local/share/com.taskmancer.app
```

---

<div align="center">
<sub>

Built in the open · [Releases](https://github.com/bogdan-tr/obelisk-suite/releases) · [Report a problem](https://github.com/bogdan-tr/obelisk-suite/issues)

</sub>
</div>
