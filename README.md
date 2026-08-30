<div align="center">

<img src="assets/obelisk.png" alt="Obelisk" width="160">

# Obelisk

**Tools for running your own life, that run entirely on your own machine.**

</div>

---

<table>
<tr>
<td width="33%" valign="top">

### Yours, and nobody else's

No account, no sync service, no telemetry. Everything lives in plain files on
your disk that you can open, back up and read without us. The only time
anything reaches the network is when you ask it to check for an update.

</td>
<td width="33%" valign="top">

### Built to look at all day

These are tools you will keep open for hours, so they are designed like it.
Careful typography, motion that helps rather than decorates, and themes with
real depth: layered backgrounds, frosted glass, light that moves.

</td>
<td width="33%" valign="top">

### Bend it to fit you

Most apps give you a colour picker and call it customisation. Here you shape
the thing itself: what the views are, what the statuses mean, what each card
shows, which panels exist. The defaults are somewhere to start.

</td>
</tr>
</table>

---

## Install

You install the launcher once. Every app comes from inside it, and uninstalls
through your system's own app list whether or not the launcher is still
around.

<details open>
<summary><b>Debian, Ubuntu, Mint</b></summary>

```bash
curl -L https://github.com/bogdan-tr/obelisk-suite/releases/download/obelisk-shell-v0.1.1/obelisk-shell_amd64.deb -o /tmp/obelisk.deb
sudo apt install /tmp/obelisk.deb
```

</details>

<details>
<summary><b>Fedora, RHEL, openSUSE</b></summary>

```bash
curl -L https://github.com/bogdan-tr/obelisk-suite/releases/download/obelisk-shell-v0.1.1/obelisk-shell_x86_64.rpm -o /tmp/obelisk.rpm
sudo dnf install /tmp/obelisk.rpm
```

</details>

<details>
<summary><b>Any Linux, without installing anything</b></summary>

```bash
curl -L https://github.com/bogdan-tr/obelisk-suite/releases/download/obelisk-shell-v0.1.1/obelisk-shell_amd64.AppImage -o obelisk
chmod +x obelisk
./obelisk
```

</details>

<details>
<summary><b>Windows and macOS</b></summary>

Both build, neither has shipped yet. There is no command here that would work
today, and a broken one seemed worse than an honest gap.

</details>

> **There is no `curl … | sh` here on purpose.**
> The usual one liner pipes a script straight into your shell. For a project
> whose whole claim is that it does not phone home, opening by asking you to
> run something you have not read would be a strange way to start. Every
> command above is short enough to read first.

---

## Taskmancer

<table>
<tr>
<td width="130" align="center" valign="top">
  <img src="assets/taskmancer.png" alt="" width="96">
  <br><sub><b>v0.1.2</b><br>available now</sub>
</td>
<td valign="top">

**Most task apps remember what you owe. This one tells you what it will cost.**

**It recommends work by rules you wrote.** Every other app buries "what should
I do now" in a hidden formula. Here you write it: weigh by priority, project,
age, urgency, whatever actually matters to you, and the answer comes back in
your own terms.

**It keeps up with your hands.** One shortcut makes a task from anywhere.
Vim motions move you through everything. You can run a whole day without
reaching for the mouse.

**It shows you the week before you get there.** Each day carries its predicted
hours against your target, so Thursday has a weight on Monday. Every chart is
yours to move, resize or throw away.

</td>
</tr>
</table>

<details>
<summary><b>More about Taskmancer</b></summary>

<br>

**Things inherit.** Projects hold subprojects, and settings flow down through
them. Set a rule where it makes sense and everything beneath it follows,
unless you say otherwise.

**Subtasks and chains.** A chain runs in order: finish one link and the next
opens itself, so a sequence you would otherwise carry in your head carries
itself.

**Tools for the tedious parts.** Work unblocks itself the moment its blocker
clears. Recurring tasks pause for a fortnight and come back with your changes
intact. Built in, not something you assemble.

**A pomodoro timer that earns its place.** Tracked time is what makes next
week's forecast true, rather than a report nobody opens.

**Plan a day against real hours.** Lay the work onto a timeline and see
whether it fits. What does not fit is the useful part. *Coming:* fitting that
work around the events already in your calendar, once Zorynda ships.

**Forty eight themes.** Cosmic, aquatic, nature, crystal, glass. The frosted
surfaces are tunable per theme: tint, blur, brightness, transparency.

**Local AI, if you want it.** An optional assistant that runs against a model
on your own machine. Off by default, and nothing leaves the room.

</details>

---

## The rest of the suite

Designed, specified, named, and not yet released. Here so you can see where
this is going.

<table>
<tr>
<td width="70" align="center"><img src="assets/zorynda.png" alt="" width="48"></td>
<td><b>Zorynda</b> · calendar<br><sub>A calendar to replace Google's, with the same navigation and theming as taskmancer.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/dreambase.png" alt="" width="48"></td>
<td><b>Dreambase</b> · dream journal<br><sub>Voice capture, tagging, and analysis that runs on your own machine.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/kupal.png" alt="" width="48"></td>
<td><b>Kupal</b> · habits<br><sub>Habit tracking without the streak guilt.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/alexandria.png" alt="" width="48"></td>
<td><b>Alexandria</b> · passwords<br><sub>A vault on your disk, with no service behind it.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/obsidian-bridge.png" alt="" width="48"></td>
<td><b>Obsidian Bridge</b> · sync<br><sub>Two way sync between the suite and an Obsidian vault.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/photos.png" alt="" width="48"></td>
<td><b>Photos</b> · library<br><sub>Your photos, searchable, without uploading them to anyone.</sub></td>
</tr>
<tr>
<td width="70" align="center"><img src="assets/alchemist.png" alt="" width="48"></td>
<td><b>Alchemist</b> · research<br><sub>Research notes that hold their shape as a project grows.</sub></td>
</tr>
</table>

---

## Updates

Apps check for their own, and the launcher notices too: a dot on the block, a
count in the corner, never a dialog in your way.

Every release is signed. Each app checks an update against a key compiled
into it and refuses anything that does not verify, so a compromised release
page cannot hand you a replacement binary.

---

## Uninstalling

Through your system's normal app list, your software centre, or
`apt remove` / `dnf remove`. The launcher hands packages to your OS installer
rather than managing them itself, so removing the launcher strands nothing.

Your data stays behind on purpose, so reinstalling picks up where you left
off. To clear that too:

```bash
rm -rf ~/.local/share/com.taskmancer.app
```

---

<div align="center">
<sub>

[Releases](https://github.com/bogdan-tr/obelisk-suite/releases) · [Report a problem](https://github.com/bogdan-tr/obelisk-suite/issues)

</sub>
</div>
