# Tessera infinity lamp

## User Guide

Version 2.0 - November 2026

---

## Contents

1. About your lamp
2. What is in the box
3. Power
4. Getting started
5. The button and the power switch
6. Connecting to the control page
7. Joining your home WiFi
8. The control page at a glance
9. Everyday controls
10. Effects
11. Colours and palettes
12. Sound and motion
13. Running on a power bank
14. Off, shut down and power saving
15. Timed schedule
16. Smart home (Home Assistant)
17. Writing your own effects
18. Firmware updates
19. Backup, reset and starting again
20. Care and cleaning
21. Troubleshooting
22. Safety notice
23. Specifications
24. Support

---

## 1. About your lamp

Your lamp is a hand-built infinity light. Addressable LEDs run along every edge
of the shape, and each face is a mirrored panel, so the light seems to fall away
into a tunnel far deeper than the lamp itself.

Inside is a small computer with its own web server. There is no app to install
and no account to create: you control it from a browser on your phone, tablet
or computer. Nothing it does depends on the internet or on a service that could
be switched off.

Depending on how it was built, your lamp may also have:

- a **microphone**, so effects can react to music and to the room,
- a **motion sensor**, so effects know which way up the lamp is and when it is
  being handled,
- a **power-bank bay**, so it keeps running from a USB-C power bank when it is
  unplugged or the mains goes off (section 13).

The lamp only shows features it actually has. If yours has no microphone, the
sound effects and sound meters are simply not there. Nothing is broken.

---

## 2. What is in the box

- The lamp
- A USB-C cable rated for the lamp's power
- [TBC: USB-C PD charger, if supplied]
- This guide and the Quick Start card

**No power bank is supplied.** The lamp runs perfectly well without one. If you
want it to run unplugged, section 13 says what to buy and how to fit it.

---

## 3. Power

### The charger

The lamp runs from a **USB-C Power Delivery (PD) charger that offers 20 V**.

> **WARNING**
> A phone charger, a laptop USB port, a car adapter or a USB hub will not run
> the lamp. It asks the charger for 20 V, and anything that cannot supply it
> leaves the lamp dark. Use a USB-C PD charger of at least **[CHARGER WATTAGE] W**,
> and a cable rated for that power.

Most laptop-style USB-C chargers of 45 W and above offer 20 V. The rating is
printed on the charger, usually as a list such as `5V 3A / 9V 3A / 15V 3A /
20V 3.25A`. Look for the 20 V entry.

### The power socket and the power switch

- **Power socket:** the USB-C socket at [TBC: socket position]. This is the only
  socket you plug the charger into.
- **Power switch:** at [TBC: switch position]. It disconnects the lamp's
  electronics from all of its power. Use it when the lamp is going into storage,
  being moved any distance, or you simply want it completely off. Section 5
  explains how it differs from the button.

[TBC: confirm whether a fitted power bank still charges while the power switch
is off.]

---

## 4. Getting started

1. Put the lamp where it will live: indoors, dry, on a firm flat surface, with
   air around it.
2. Plug the charger into the wall, and the cable into the lamp's power socket.
3. Set the power switch to **ON**.

The lamp starts a few seconds later, in whatever state it was in when it was
last used. The first time, it starts lit and showing an effect.

### Where to put it

- Indoors, out of direct sunlight, away from radiators.
- On a firm, flat surface. It is heavier than it looks, and the panels are
  rigid.
- Not in a closed cabinet, under a cloth or against a curtain.

---

## 5. The button and the power switch

### The button

There is one button, on the base. It does everything you need day to day.

| Action | Result |
|---|---|
| Press | Next effect |
| Double press | Previous effect |
| Hold about 1 second, then let go | LEDs on or off |
| Hold 3 seconds, until the LEDs flash amber | Shut down |
| Hold about 1 second while shut down | Wake up |

The button skips any effect your lamp cannot run, so on a lamp with no
microphone a press never lands on a sound effect that would leave it dark.

### Three ways to switch off

| | What switches off | What keeps working | How to switch back on |
|---|---|---|---|
| **Off** (1 second hold, or the On/Off button on the page) | The LEDs | WiFi, the control page, Home Assistant, the schedule | The button, the page, Home Assistant or the schedule |
| **Shut down** (3 second hold, or Shut down on the page) | The LEDs, WiFi and the lamp's computer | Nothing. The lamp draws almost nothing | Hold the button for about 1 second |
| **Power switch OFF** | Everything | Nothing. The lamp draws no power at all | Power switch ON |

**Off** is what you want most of the time: the lamp is dark but still listening,
so your phone, your schedule and your smart home can all bring it back.

**Shut down** is for when the lamp will not be used for a while but you want to
leave it plugged in, or when it is running on a power bank and you want the bank
to last (section 13). While shut down nothing can reach it over the network.

The **power switch** is the hardware off. Use it for storage, before moving the
lamp, and whenever you want certainty that it is drawing nothing.

---

## 6. Connecting to the control page

The lamp has no app. Its control page is a web page that the lamp serves itself.

### First time, or any time it is not on your WiFi

The lamp broadcasts its own WiFi network.

1. Open **WiFi settings** on your phone, tablet or laptop.
2. Join the network called **`infinity-lamp`**. It has no password.
3. The control page should open by itself. If it does not, open a browser and
   go to **http://infinity.lamp** or **http://192.168.4.1**.

Your device will warn that this network has no internet. That is expected: the
lamp is not a router. Some phones switch back to mobile data when they see
this. If the page stops responding, turn mobile data off while you set up.

### Once it is on your home WiFi

Open a browser on any device on the same network and go to:

**http://infinity-lamp.local**

If that does not load (some older Android devices and some work networks do not
understand `.local` names), find the lamp in your router's list of connected
devices, where it appears as `infinity-lamp`, and use its IP address instead.
Giving it a fixed address with a DHCP reservation on your router is worth the
two minutes; the Network panel shows the lamp's MAC address for this.

You can have the page open on several devices at once. They all stay in step.

---

## 7. Joining your home WiFi

On the control page, find the **Network** panel.

1. Under *Your WiFi network*, enter your network name and password.
2. Optionally change the **Hostname** under *Identity*. This is the lamp's name
   on your network and sets its address: a hostname of `lounge-lamp` makes it
   **http://lounge-lamp.local**. If you have more than one lamp, give each its
   own.
3. Press **Save network settings**, then **Reboot device**.

**Network changes only take effect after a restart.** Saving alone changes
nothing you can see, which looks like a failure and is not.

Notes:

- Once the lamp has joined your WiFi its own `infinity-lamp` network switches
  off, so several lamps in one house do not clutter your WiFi list.
- If your WiFi disappears for long enough, the lamp puts its own network back up
  so you can always reach it, and takes it down again when your WiFi returns.
- The lamp uses **2.4 GHz WiFi only**. A router that offers 2.4 GHz and 5 GHz
  under one name is fine. If it has a separate 5 GHz-only name, use the other
  one.
- To rename the lamp on screen, click its name in the top-left corner of the
  page. That is a display label only: it does not change the address.

---

## 8. The control page at a glance

There are two pages.

| Page | What is on it |
|---|---|
| **Lamp page** (the one you land on) | Lamp controls, effects, colour palette, your own effects, power readings, schedule |
| **Advanced settings** (link at the top) | How the lamp was built and connected: LED layout, sensors, network, smart home, power hardware, firmware updates, backup and reset |

Everyday use only needs the lamp page.

Across the top of both pages is a **header** that stays in view as you scroll.
It holds:

- the **lamp name** (click it to rename the lamp),
- an **On/Off** button and a **brightness** slider,
- small readouts, each shown only if your lamp has the part behind it:
  - sound meters and `MIC`, if a microphone is fitted,
  - `TILT` and `STILL`, if a motion sensor is fitted,
  - `FX` and `PAL`, the effect and palette playing now,
  - `LEDS`, an estimate of what the LEDs are drawing, in watts then amps,
  - `LAMP`, the measured power of the whole lamp,
  - the power bank's charge, when the lamp is running on one.

Anything the lamp cannot measure is hidden rather than shown blank, so
everything you can see is a real reading.

---

## 9. Everyday controls

Everything in **Lamp controls** takes effect and is saved the moment you change
it. There is no Save button in this section.

### Power

**Power** switches the LEDs on and off. The lamp stays connected either way.

### Brightness

A 0-100% slider. **100% is the most this lamp is set to run at**, which is
deliberately below what the LEDs could draw flat out. It keeps the lamp cool,
keeps the colours accurate and keeps a power bank going for longer.

Brightness 0% saves as much power as switching off, but does not move the Power
switch, so sliding back up brings the light straight back.

### Effect speed

Speeds up or slows down whatever effect is playing. Some effects show it more
than others.

### Shut down

Switches the lamp off completely. See section 14.

### Turn the bottom panel off when the lamp sits still

On lamps with a motion sensor. Once the lamp has not moved for a few seconds,
it works out which face is resting on the surface and turns that face off. You
cannot see it, so the lamp looks the same, but it saves power and stops the base
glowing onto the shelf. Pick the lamp up and the face comes straight back.

### Auto-cycle

Steps through the effects on its own, every 30 seconds unless you change it.
You choose which **groups** take part:

- Always available
- Sound reactive
- Motion reactive
- Sound + motion
- Your effects

Tick only *Sound reactive*, for example, to cycle just the music effects.
Unticked groups can still be chosen by hand. A line underneath says how many
effects will actually cycle.

Auto-cycle pauses while the lamp is off and carries on from the same effect when
it comes back on.

---

## 10. Effects

There are **34 built-in effects**. Tap one to play it.

They are grouped by what drives them, and each tile carries its group's colour
on its left edge. **A group that needs a sensor your lamp does not have is
hidden.** A lamp without a microphone shows 26 effects, not 34 with eight dead
ones.

### Always available

Need no sensor. Work on every lamp.

| Effect | What it does |
|---|---|
| Rainbow Flow | The full spectrum flowing around the shape |
| Comet Chase | A bright head with a fading tail, chasing round the edges |
| Twinkle | Random points slowly brightening and fading |
| Plasma | Soft, slow, organic blobs of colour |
| Fire | Flickering flame rising from the base |
| Edge Runner | A single point running edge to edge |
| Breathe | The whole lamp slowly rising and falling in brightness |
| Solid / Gradient | One colour, or a smooth blend of your palette |
| Gradient Sweep | Your palette sliding across the shape |
| Colour Wipe | Each colour painting itself on in turn |
| Theatre Chase | A classic marquee chase |
| Confetti | Scattered, short-lived flecks of colour |
| Meteor | A falling streak with a decaying trail |
| Juggle | Coloured dots weaving through each other |
| Aurora | Slow drifting curtains of colour |
| Matrix Rain | Falling columns of code-rain |
| Panel Plasma | Plasma worked out per face rather than per edge |
| Ripple | Rings spreading from a moving point |
| Face Cycle | Lights one face at a time |

*Matrix Rain, Panel Plasma, Ripple and Face Cycle are designed for lamps with
LED panels on the faces. On an edge-lit lamp they still run, but look flatter.*

### Sound reactive

Need the microphone. The lamp listens to the room; there is nothing to plug in.

| Effect | What it does |
|---|---|
| VU Meter | A level meter climbing the shape |
| Spectrum | Bass to treble mapped around the lamp |
| Beat Pulse | The whole lamp pulses on the beat |
| Bass Bloom | A level that swells with the bass, with treble glitter above it |
| Sound Ripple | Each beat sends a ring travelling right across the lamp |
| Audio Sparkle | Sparkle that follows the volume, sharpened by the treble |
| Beat Strobe | A different slice of the lamp fires on each beat |

### Motion reactive

Need the motion sensor. Pick the lamp up and turn it.

| Effect | What it does |
|---|---|
| Rain | Droplets that always fall towards whatever is currently down |
| Gravity Fill | The lamp fills like a glass, level however you hold it |
| Spirit Level | A bright band along true horizontal, rolling as you tilt |
| Tilt Flow | Liquid that sloshes and settles rather than snapping to the new angle |
| Gravity Pointer | A pool of light at whichever part is lowest |
| Shake Sparkle | Sparkles burst when the lamp is picked up or shaken, then fade |
| Orientation Hue | The colour follows which way the lamp is leaning |

### Sound + motion

| Effect | What it does |
|---|---|
| Tilt Spectrum | Spectrum, with the bands staying level however the lamp is turned |

### Your effects

Effects you have written yourself (section 17). Tap one to play it, or click it
to open its formulas in the editor.

### What each effect uses

Below the effect grid is a table listing every effect the lamp knows, including
any it cannot run, with what each one needs. The grid shows what your lamp can
do; the table is the complete list.

---

## 11. Colours and palettes

A **palette** is a list of colours. One colour gives a solid; several give a
gradient that the effects blend through.

1. Pick a **Preset**, or edit the colours directly with **Add colour** and
   **Remove**.
2. Press **Apply palette**.
3. Press **Save current** to keep it under a name of your own. Under **Saved
   palettes**, pick one and press **Load** to use it again, or **Delete** to
   remove it.

Some effects carry their own colours and ignore the palette: Rainbow Flow, Fire,
VU Meter, Spectrum, Orientation Hue and Tilt Spectrum. The *What each effect
uses* table says which.

---

## 12. Sound and motion

### Sound

The microphone listens to the room, so anything you can hear the lamp can react
to: a speaker, a TV, a conversation, applause.

- Sound effects look best within a few metres of the speaker, at a normal
  listening volume.
- The lamp adjusts to the room's background level by itself. Give it a few
  seconds after the music starts, and again after it stops.
- If it seems deaf, clap and watch the sound meters in the header. If they
  move, the microphone is fine and it is the volume or the effect. If they do
  not, see *Sensors* on the Advanced settings page.
- Nothing is recorded, stored or sent anywhere. The sound is reduced to four
  numbers (level, bass, mid and treble) and thrown away, and the microphone is
  paused while the lamp is off.

### Motion

The motion sensor tells the lamp which way is down and whether it is being
handled. It drives the motion effects, Shake Sparkle, and the power saving that
turns off the face resting on the table.

If the tilt effects seem to lean when the lamp is sitting normally, calibrate
it: on the Advanced settings page, under *Sensors & calibration*, stand the lamp
upright where it normally lives, leave it still for a couple of seconds, and
press **Calibrate level**. It is remembered across restarts.

---

## 13. Running on a power bank

*Lamps with a power-bank bay only.*

A USB-C power bank in the bay turns the lamp into a portable light, and keeps it
running through a power cut.

### How it works

- **While the lamp is plugged in**, it runs from the mains and charges the bank
  gently in the background, whether the LEDs are on or off.
- **When you unplug it, or the mains goes off**, it switches over to the bank by
  itself.
- **When you plug it back in**, it goes back to the mains and starts charging the
  bank again.

At the switch-over the LEDs blink off for up to a second while the lamp asks the
bank to stop charging and start supplying. The lamp itself and the control page
stay up throughout. This is normal and not a fault.

On the bank the lamp runs a little less bright at the top of the slider, to make
the bank last. That is deliberate.

### Choosing a bank

The lamp does not come with a bank. Any bank that meets all of these will work:

| Requirement | Why |
|---|---|
| **USB-C Power Delivery output that offers [BANK PD VOLTAGE] V** | The lamp asks the bank for this voltage. A bank that only gives 5 V cannot run it. Check the output list on the bank or its listing, for example `5V 3A / 9V 2.22A / 12V 1.67A` |
| **20 W or more** | The bank's wattage limits how bright the lamp can run on battery |
| **UKCA or CE marked, from a proper retailer** | It is the only part of the lamp with cells in it. Avoid marketplace listings with impossible capacity claims |
| **Fits the bay: [BAY DIMENSIONS]** | A typical 10,000 mAh bank is about 140 x 70 x 26 mm |

One USB-C port is enough. The bank does not need two ports, and it does not
need pass-through charging.

As a rough guide, a 10,000 mAh bank runs a typical lamp for **about 4 hours** at
everyday brightness. Bright white uses far more than a deep colour, because
white lights all three colours in every LED at once.

### Fitting the bank

1. Unplug the lamp from the mains and set the power switch to **OFF**.
2. [TBC: open the bay - how the bay opens.]
3. Plug the bay's USB-C lead into the bank's **USB-C** port.
4. Seat the bank in the bay and close it.
5. Set the power switch to **ON** and plug the lamp back into the mains.

Leave it plugged in until the bank is full the first time. The lamp charges the
bank gently, so a large bank can take a day or more from empty; the bank's own
charge lights show its progress.

### What the Power panel shows

The **Power** panel on the lamp page shows the source (mains or battery), the
power the lamp is using, and the bank's state: *not connected*, *charging*,
*fully charged* or *in use*.

The lamp cannot see inside a sealed bank, so it measures it instead. **After the
bank has been fully charged through the lamp**, the lamp counts the energy taken
out of it. The first time the bank runs from full to empty, the lamp learns how
much that bank really delivers. From then on the Power panel and the header show
the charge left and the time remaining, as real measurements. Until then they say
*learning*, which is normal.

If you swap banks, or charge the bank somewhere else, the lamp starts again from
the next full charge.

### Off on a power bank

A power bank switches its output off when nothing seems to be drawing from it.
To stop that happening, **the lamp keeps drawing a little current whenever it is
running on the bank, even when it is switched Off.** Otherwise the bank would cut
the power and take the controls with it.

So a lamp left Off on the bank slowly empties it. Three ways to deal with that:

- **Plug the lamp back into the mains** when you have finished with it. This is
  the normal case.
- **Shut it down** (hold the button for 3 seconds). The lamp stops drawing, the
  bank switches itself off, and nothing more is taken from it. To switch back on,
  wake the bank first (press its own button, or plug the lamp into the mains),
  then within 60 seconds hold the lamp's button for about 1 second.
- **Let it happen automatically.** On the Advanced settings page, under *Power
  saving & standby*, set **Let the bank sleep after** to a number of minutes.
  After that long switched Off on the bank, the lamp lets the bank switch itself
  off.

A notice on the Power panel explains this whenever the lamp is running on its
bank.

### Looking after the bank

- Follow the bank's own instructions, and replace it if it is damaged, swollen
  or gets hot.
- For storage of more than a month, take the bank out, or set the power switch
  to OFF.
- At the end of its life, take the bank to a battery recycling point, never the
  household bin. Supermarkets, DIY shops and council recycling centres take them
  free of charge.

---

## 14. Off, shut down and power saving

### Off

The LEDs go dark, but the lamp stays awake so the control page, your smart home
and the schedule keep working. While it is off it slows itself down and
throttles its WiFi, and draws a small fraction of its running power.

### Shut down

Shut down switches the LEDs, WiFi and the lamp's computer off, and the lamp
draws almost nothing.

- **To shut down:** press **Shut down** on the lamp page, or hold the button for
  3 seconds until the LEDs flash amber, then let go.
- **To switch back on:** hold the button for about 1 second. A shorter press is
  ignored, so a knock on the shelf does not wake it. It comes back on, showing
  the effect it had before.
- While it is shut down, the control page, Home Assistant, the schedule and
  update checks are all unavailable. Nothing can switch it on over the network.
- Plugging a shut-down lamp into the mains does not switch it on. It stays shut
  down until you hold the button.
- It cannot shut down while a firmware update is being installed.

### The power switch

The power switch cuts all power to the lamp's electronics. Use it for storage
and before moving the lamp.

### Power-saving settings

Three savings are on by default and worth leaving on:

- **WiFi power saving.** The biggest saving. The first tap after a quiet spell
  can take a moment longer to respond.
- **A slower processor and frame rate while the LEDs are off.**
- **The bottom panel off when the lamp sits still** (lamps with a motion sensor,
  section 9).

They are on the Advanced settings page under *Power saving & standby*, with a
**Standby glow** option that holds the lamp at a very dim level when it is Off.
It looks nice, but cancels most of the saving.

---

## 15. Timed schedule

On the lamp page, under **Schedule (auto on/off)**.

1. Tick **Enable schedule**.
2. Pick your **Region**. The UK entry handles GMT and BST by itself.
3. Add rules with **Add rule**. Each rule is an action (turn on or turn off), a
   time, and the days it applies to. Tap the days to pick them; no days picked
   means every day.
4. Press **Save schedule**.

Each rule runs once, at its time, so you can still switch the lamp by hand in
between: turning it off at 21:00 does not stop you turning it back on at 21:05.
After a restart the lamp switches to whatever the schedule says it should be
doing at that moment.

The lamp gets the time from the internet once it is on your WiFi. **The schedule
only works on a network with internet access.** On its own network the lamp has
no clock. A shut-down lamp does not follow the schedule.

---

## 16. Smart home (Home Assistant)

The lamp speaks **MQTT** and supports Home Assistant's automatic discovery. If
that means nothing to you, skip this section. Nothing here is needed for normal
use.

On the Advanced settings page, in **MQTT & Home Assistant**:

1. Tick **Enable MQTT** and leave **Home Assistant discovery** ticked.
2. Enter your broker's address, port, username and password.
3. Press **Save & connect**. The status line shows when it is connected.

The lamp then appears in Home Assistant with:

- a **light**, with on/off, brightness, an effect list that includes your own
  effects, and a colour picker that sets the palette to that colour,
- an **effect** selector,
- a **palette** selector listing your saved palettes.

It reports every change as it happens, including ones made with the button, so
Home Assistant always matches the lamp.

---

## 17. Writing your own effects

The lamp has a built-in effect editor. You write three formulas, one for each
part of the colour, and the lamp works them out for every LED many times a
second. There is nothing to install and no reprogramming.

1. On the lamp page, under **Create effect (expression editor)**, press **Open
   the expression editor**.
2. Give it a **Name**, and choose the **Output mode**: **HSV** (hue, saturation,
   brightness) or **RGB** (red, green, blue).
3. Type your three formulas. **Speed** sets how fast this effect runs, on top of
   the main speed slider.
4. Press **Validate** to check the formulas for mistakes.
5. Press **Save effect**. It appears in the effect grid under *Your effects*; tap
   it to see it on the lamp. **New / clear** starts again with an empty editor.

The **Worked examples** underneath load ready-made formulas to learn from. Each
formula gives a number from 0 to 255.

**Values you can use**

| Name | Meaning |
|---|---|
| `i` | LED number |
| `n` | Total number of LEDs |
| `p` | Position along the chain, 0 to 1 |
| `t` | Time in seconds |
| `x y z` | Position in space |
| `h` | Height, 1 at the top |
| `e` | Edge number |
| `rnd` | A fixed random number for each LED, 0 to 1 |
| `a` | Overall sound level |
| `bass mid treble` | The sound bands |
| `beat` | 1 on a beat, otherwise 0 |
| `gx gy gz` | Which way gravity points |

**Functions**

`sin cos tan abs sqrt floor ceil frac sign exp log tri noise`,
`min max mod pow atan2 hypot step`, `clamp(x,lo,hi)`, `select(cond,a,b)`,
`lerp(a,b,t)`, and `pr(u) pg(u) pb(u)`, which read colours from your current
palette.

Operators: `+ - * / % ^` and comparisons `< > <= >= ==`.

**Examples**

```text
# Audio rainbow tunnel
hue: i*8 + t*40 + bass*120
sat: 255
val: 128 + 120*sin(p*6.28 - t*3) * (0.3 + a)

# Sparkle weighted to the top
hue: 160
sat: 120
val: 255 * step(0.85, noise(i*0.3 + t*2))

# Horizon that follows the tilt - brightest where the lamp points down
hue: 150
sat: 200
val: clamp(180 * (x*gx + y*gy + z*gz) + 40, 0, 255)
```

Your effect files itself into the right group: use `a`, `bass`, `mid`,
`treble` or `beat` and it becomes a sound effect; use `gx`, `gy` or `gz` and it
becomes a motion effect.

---

## 18. Firmware updates

The lamp's software is updated over WiFi. Your settings, palettes and own
effects are kept.

- Once the lamp is on your WiFi it checks for updates by itself, once a day by
  default. **It only ever tells you about an update; it never installs one on
  its own.**
- To check or install by hand: Advanced settings, **Firmware and updates**,
  **Check for updates**, then **Install update** if one is offered. The LEDs show
  a progress bar and the lamp restarts when it has finished.
- Leave the lamp plugged in to the mains while it updates. If the power drops
  halfway, the lamp still starts on its previous version.
- No internet on the lamp? Download the release files from
  [github.com/infinity-lamps/tessera/releases](https://github.com/infinity-lamps/tessera/releases)
  and use **Upload a .bin file** under *Firmware and updates*.

The page shows the version running now. Quote it if you ever need to ask for
help.

---

## 19. Backup, reset and starting again

All on the Advanced settings page, under **Backup and provisioning**.

### Backup

- **Export config** downloads a file containing everything: palettes, your own
  effects, the schedule and the lamp's build settings. Keep a copy, especially
  after writing effects you would be sad to lose.
- **Export with passwords** includes your WiFi and MQTT passwords in plain text.
  Only use it if you need it, and store the file carefully.
- **Import** puts a file back.

### Reset

**Reset** returns the lamp to the way it was built and tested: the right shape,
LED count and layout for your lamp, not a generic default. It discards your
palettes, own effects, schedule and smart-home settings. There is no undo, so
export first.

**Keep network settings** is ticked by default, so the lamp stays on your WiFi at
the same address. Untick it only when passing the lamp on to someone else; it
will then come back on its own `infinity-lamp` network.

### Settings to leave alone

The rest of the Advanced settings page describes **how the lamp is physically
built**: shape, LED count, colour order, which strip runs along which edge, and
which power parts are fitted. Changing them makes the lamp show nonsense until
they are put back. They are there so the lamp can be repaired or rebuilt, and
the export file covers them all.

If you have changed something and cannot get back, press **Reset** with **Keep
network settings** ticked. Nothing you can do from the control page can
permanently damage the lamp.

---

## 20. Care and cleaning

- **Panels:** a dry microfibre cloth, lightly. The mirrored surfaces scratch
  easily, and a scratch shows as a bright streak in the tunnel.
- **Never use** glass cleaner, alcohol, solvents, kitchen sprays or abrasive
  cloths. Ammonia and alcohol both craze acrylic.
- **Dust:** a soft brush or a puff of air first, so you do not wipe grit across
  the panels.
- **Storage:** upright, dry, at room temperature, with the power switch OFF. Take
  a power bank out if it will be stored for more than a month.
- **Do not** take the lamp apart, get it wet or use it outdoors.

---

## 21. Troubleshooting

| Symptom | What to do |
|---|---|
| Nothing lights up | Check the power switch is ON. Check it is a **USB-C PD** charger that offers 20 V, with a suitable cable. Hold the button for about 1 second, in case it is off or shut down |
| Lamp is on but dim | Check the brightness slider. On a power bank, the top of the range is deliberately a little lower |
| LEDs blink off for a moment when the mains goes | Normal on lamps with a power bank: the lamp is switching to the bank |
| It will not run unplugged | Check a bank is fitted, its lead is plugged into its USB-C port, and it is charged. Check it meets the rules in section 13 |
| Power panel says the bank is *not connected* | Reseat the bank's lead. A bank that has emptied itself completely may need waking with its own button |
| Bank charge shows *learning* | Normal until the bank has been fully charged through the lamp and run down once (section 13) |
| Lamp will not switch on after a shut down | Hold the button for a full second. On a bank, wake the bank first, then hold the button within 60 seconds |
| Cannot find the `infinity-lamp` network | It is probably already on your home WiFi. Try **http://infinity-lamp.local**, or look for it in your router's device list |
| `infinity-lamp.local` does not load | Your device may not support `.local` names. Use the lamp's IP address from your router |
| Page loads but does not respond | Reload it. With WiFi power saving on, the first tap after a quiet spell can take a moment |
| Page stops responding during setup | Your phone may have switched to mobile data. Turn mobile data off while connected to `infinity-lamp` |
| Some effects are missing | Your lamp was built without that sensor. The *What each effect uses* table says which part each needs |
| Sound effects do not react | Clap and watch the header's sound meters. If they move, turn the music up or move the lamp nearer. If not, see *Sensors* on the Advanced settings page |
| Motion effects lean the wrong way | Run **Calibrate level** (section 12) with the lamp sitting where it normally lives |
| One face is dark when the lamp sits still | That is the power saving working. Pick the lamp up |
| Effect changes by itself | Auto-cycle is on. Untick it in Lamp controls |
| The schedule does nothing | The lamp needs your WiFi and the internet to know the time. Check **Enable schedule** is ticked and saved |
| It restarts or flickers on bright effects | The charger is not supplying enough power. Use a PD charger of at least [CHARGER WATTAGE] W and a cable rated for it |
| One section is dark or the wrong colour | Usually a connection inside that has worked loose. Do not open the lamp; get in touch (section 24) |
| Lost after changing settings | Advanced settings, **Reset**, with **Keep network settings** ticked |

If none of this helps, get in touch (section 24). It is far easier for me to fix
than for you to guess.

---

## 22. Safety notice

**Please read this section.**

### This is a hand-built lamp

Your lamp was designed, built and tested by one person. [TBC: certification
status - UKCA / CE marking and the terms it is supplied under.] Until that is
confirmed, treat it as a hand-made item for private, indoor, domestic use.

### Electrical

- Indoor, dry locations only.
- Use a USB-C PD charger from a reputable maker, of at least [CHARGER WATTAGE] W.
- Do not use the lamp with any part of it removed or damaged.
- Set the power switch to OFF before moving the lamp any distance, and when you
  are away for a long period.

### Power bank (lamps with a bay)

- Use only a finished, UKCA or CE marked USB-C PD power bank that meets section
  13, bought from a proper retailer.
- Never use a bank that is damaged, dented, swollen, or has been dropped hard.
- Do not leave the lamp in a car, in direct sunlight or near a radiator.
- Do not charge it on soft furnishings, and avoid leaving it charging unattended
  overnight if you can.
- **If the lamp or the bank becomes hot, swells, hisses or smells sharp or
  sweet:** unplug it, set the power switch to OFF if you can do so safely, move
  it somewhere non-flammable away from anything that can burn, do not put it in
  water, and contact me. Do not put it in the bin.
- At the end of its life the bank goes to a battery recycling point, never the
  household bin.

### Flashing light

Some effects flash or strobe quickly, in particular **Beat Strobe**, **Beat
Pulse** and **Theatre Chase**. A small proportion of people can have seizures
triggered by flashing light. If you or anyone in your home is photosensitive,
avoid those effects, and avoid Auto-cycle, which will eventually reach them, or
untick its *Sound reactive* group.

At full brightness the LEDs are uncomfortable close up. Do not stare into them.

### General

- Not a toy. Keep it away from young children and from pets that knock things off
  shelves. It is heavy and the panels are rigid.
- Do not cover the lamp or block the air around it.
- Do not open it, modify the wiring, or use a charger that is not USB-C PD.
- At the end of its life the lamp is electrical waste: take it to an electrical
  recycling point, not the household bin.

---

## 23. Specifications

| | |
|---|---|
| Model | [EDGE LENGTH] mm [SHAPE] |
| Serial number | [SERIAL] |
| Overall size | [DIMENSIONS] |
| Weight | [WEIGHT] |
| LEDs | [LED COUNT], individually addressable |
| Controller | ESP32-S3, dual core, with WiFi |
| Network | 2.4 GHz WiFi (802.11 b/g/n), plus its own network for setup |
| Control | Built-in web page, the button, MQTT. No app, no cloud, no account |
| Sensors fitted | [MICROPHONE / MOTION SENSOR / NONE] |
| Power input | USB-C Power Delivery, 20 V, [CHARGER WATTAGE] W minimum |
| Power switch | Yes, full hardware off |
| Power bank | [NONE / Bay for an owner-supplied USB-C PD bank, [BAY DIMENSIONS]] |
| Bank requirement | USB-C PD output offering [BANK PD VOLTAGE] V, 20 W or more |
| Bank charging | From the lamp, 5 V, up to 1.5 A, while plugged in |
| Typical power | [X] W lit, under [Y] W off, almost nothing shut down |
| Built-in effects | 34, plus unlimited effects of your own |
| Smart home | MQTT with Home Assistant discovery |
| Firmware | Open source (MIT), updated over WiFi |

---

## 24. Support

**Made by Ryan in Scotland**

- Email: **[SUPPORT EMAIL]**
- Guides, firmware and replacement-part print files:
  **[infinity-lamps.github.io/tessera](https://infinity-lamps.github.io/tessera/)**
- Report a problem:
  **[github.com/infinity-lamps/tessera/issues](https://github.com/infinity-lamps/tessera/issues)**

If something has gone wrong, please tell me:

- the model and serial from the label underneath,
- the firmware version, shown under *Firmware and updates*,
- what the lamp is doing, and what the header and Power panel say,
- whether it is on mains or on a power bank,
- what you changed most recently, if anything.

The power-bank bay is yours to open, and nothing else is. There is nothing else
inside you can service, the wiring is easy to disturb, and I would much rather
fix it than have it become an ornament.

---

*Tessera infinity lamp. Flat faces, infinite depth.*
