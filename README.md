<div align="center">

<img src="assets/obelisk.png" alt="Obelisk" width="160">

# Obelisk

**A suite of tools for running your own life — and none of it leaves your machine.**

</div>

---

<table>
<tr>
<td width="33%" valign="top">

### Fully local, private by default

There is no account, no sync service and no telemetry. Your tasks are files,
your settings are JSON, and both sit on your own disk. The only time anything
touches the network is when you ask it to check for an update. If this
project vanished tomorrow you would still have everything, in formats you can
open.

</td>
<td width="33%" valign="top">

### Designed, not assembled

Every app is built to be looked at for hours without tiring you. Real
typographic hierarchy, motion that clarifies rather than decorates, and
dozens of themes that were designed rather than generated — layered
backgrounds, gaussian-blurred glass, and light that moves.

</td>
<td width="33%" valign="top">

### Customisation that goes deep

Not a colour picker bolted onto someone else's decisions. Your own statuses,
priorities, views, cards, keybindings and layouts — down to what each card
shows and which panels exist at all. The defaults are a starting point, not
a cage.

</td>
</tr>
</table>

---

## Install

The launcher is the only thing you install by hand. Every app is installed
from inside it, and uninstalls through your system's own app list whether or
not the launcher is still around.

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

Not published yet. Both build in CI; neither has been released, so there is
no command here that would work today.

</details>

> **Why there is no `curl … | sh` here.**
> The usual one-liner pipes a script straight into your shell. For a project
> whose entire claim is that it does not phone home, opening by asking you to
> execute an unread remote script would be the wrong first thing to ask.
> Every command above is one you can read in full before you run it.

---

## Taskmancer

<table>
<tr>
<td width="130" align="center" valign="top">
  <img src="assets/taskmancer.png" alt="" width="96">
  <br><sub><b>v0.1.1</b><br>available now</sub>
</td>
<td valign="top">

**Most task apps remember what you owe. This one tells you what it will cost.**

**Task recommendation you actually control.** Other apps decide what matters
with a priority field and a hidden formula. Here you write the rules: weight
by priority, project, staleness or urgency, in cards you define, so "what
should I do now" is answered the way *you* would answer it — not the way a
product manager guessed.

**A keyboard that keeps up with you.** `Ctrl+T` creates a task from anywhere
in the app, including inside a chain, inheriting that chain's defaults. Vim
motions move you through lists, boards and chains without reaching for the
mouse.

**Analytics that change what you do next.** Not a dashboard you visit once.
The week strip shows every day's predicted hours against your own target, so
next Thursday has a weight before Thursday arrives — and every widget is
movable, resizable and yours to arrange.

</td>
</tr>
</table>

<details>
<summary><b>More about Taskmancer</b></summary>

<br>

**Nesting and inheritance.** Projects hold subprojects, and settings flow
down through them — defaults, rules and card behaviour are set once at the
level that makes sense and inherited everywhere below. Change the parent and
the children follow, unless you have told one of them otherwise.

**Subtasks and chains.** A subtask belongs to its parent. A chain runs in
order — finish one link and the next opens itself, so a sequence you would
otherwise hold in your head holds itself.

**Tools that do the tedious part.** Auto-unblock moves work forward the
moment its blocker clears. Pause recurring tasks suspends a series for a
fortnight and resumes it without losing what you changed. They are built in,
not automations you have to assemble.

**A pomodoro timer that feeds the forecast.** Tracked time is not a report
you never read — it is what makes next week's number true.

**Plan view.** Lay a day's work onto real hours and see whether it fits; what
does not fit is the useful part. *Coming:* scheduling project work into the
gaps between events in your actual calendar, once Zorynda ships.

**Forty-eight themes.** Across cosmic, aquatic, nature, crystal and glass
families — with gaussian-blurred surfaces you can tune per theme: tint,
blur, brightness and transparency, each on its own slider.

**Local AI, experimental.** An optional assistant that runs against a model
on your own machine. Off by default, and it never sends your tasks anywhere.

</details>

---

## The rest of the suite

Each of these has a design, a specification and a name. None has a release
yet — they are listed so you can see where this is going, not as a promise
about when.

<table>
<tr>
<td width="70" align="center"><img src="assets/zorynda.png" alt="" width="48"></td>
<td><b>Zorynda</b> · calendar<br><sub>A fully local calendar built to replace Google Calendar, with vim-motion navigation and taskmancer-grade theming.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/dreambase.png" alt="" width="48"></td>
<td><b>Dreambase</b> · dream journal<br><sub>Voice capture, auto-tagging and analysis that runs on your own machine, with Obsidian import.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/kupal.png" alt="" width="48"></td>
<td><b>Kupal</b> · habits<br><sub>Habit tracking without the streak guilt.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/alexandria.png" alt="" width="48"></td>
<td><b>Alexandria</b> · passwords<br><sub>A vault that stays on your disk, with no service behind it.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/obsidian-bridge.png" alt="" width="48"></td>
<td><b>Obsidian Bridge</b> · sync<br><sub>Two-way sync between the suite and an Obsidian vault.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/photos.png" alt="" width="48"></td>
<td><b>Photos</b> · library<br><sub>Your library, on your disk, searchable without uploading it to anyone.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/alchemist.png" alt="" width="48"></td>
<td><b>Alchemist</b> · research<br><sub>Research notes that hold their shape as a project grows.</sub></td>
</tr>
</table>

---

## Updates

Each app checks for its own updates, and the launcher notices them too — a
dot on the app's block and a count in the header, never a dialog in your way.

Updates are **signed**. Every app verifies a release against a public key
compiled into it and refuses anything that does not check out, so a
compromised release page cannot hand you a replacement binary.

---

## Uninstalling

Through your system's normal app list, your distribution's software centre,
or `apt remove` / `dnf remove`. The launcher hands packages to your OS
installer rather than managing them itself, so removing the launcher strands
nothing.

Your data is deliberately left behind, so reinstalling picks up where you
left off. To remove that too:

```bash
rm -rf ~/.local/share/com.taskmancer.app
```

---

<div align="center">
<sub>

[Releases](https://github.com/bogdan-tr/obelisk-suite/releases) · [Report a problem](https://github.com/bogdan-tr/obelisk-suite/issues)

</sub>
</div>
