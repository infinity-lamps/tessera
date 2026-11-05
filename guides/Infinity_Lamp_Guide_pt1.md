# Infinity Lamp

## Quick Start

Welcome to your Infinity Lamp. It is a hand-built, WiFi-connected light with
34 built-in effects, a browser-based control panel, and sensors that let it
react to sound and to being picked up.

This card gets you lit in five minutes. The full **User Guide** covers
everything else.

---

### 1. Fit the batteries (battery models)

**The lamp ships with an empty battery bay and no cells.** It runs on mains with
the bay empty, so this step can wait if you want to.

You need **three flat-top, unprotected 18650 cells**, same make, model and age,
from a reputable seller. Samsung INR18650-35E is the cell to buy. **Protected
cells are too long and will not fit.**

1. Unplug USB-C. Switch the battery bay isolator **off**.
2. Check each cell reads at least 3.0 V and all three are within 50 mV of each
   other.
3. Fit the cells, checking the polarity of every one.
4. Switch the isolator **on**, then plug USB-C back in.

**User Guide section 3** has the full detail, including what to do if the lamp
says it is not charging.

---

### 2. Plug it in

Use the supplied USB-C charger and cable.

> **Important:** the lamp needs a **USB-C Power Delivery (PD)** charger. A
> standard 5 V phone charger, a laptop USB port or a car socket will not run it
> and will not charge it. If you replace the charger, it must be a USB-C PD
> unit of at least **[CHARGER WATTAGE] W**.

If you have fitted cells, leave the lamp plugged in for the first **[FIRST
CHARGE HOURS] hours** before running it unplugged.

The lamp switches on by itself a few seconds after power is applied.

---

### 3. Use the button

There is one button on the base.

| Action | What it does |
|---|---|
| **Short press** | Next effect |
| **Press and hold** (about 1 second) | Lamp on / off |

That is the whole physical interface. Everything else is on the web page.

---

### 4. Open the control page

The lamp creates its own WiFi network the first time it is switched on.

1. On your phone, tablet or laptop, open **WiFi settings**.
2. Join the network named **`infinity-lamp`**. There is no password.
3. A control page should open by itself. If it does not, open a browser and go
   to **http://infinity.lamp** (or **http://192.168.4.1**).

You now have full control: power, brightness, speed, effects and colours.

---

### 5. Put it on your home WiFi (optional but recommended)

Joining your home network means you can control the lamp from any device in the
house without switching WiFi networks, and it enables the clock-based schedule.

1. On the lamp's control page, scroll to the **Network** panel.
2. Enter your WiFi name and password. Press **Save**.
3. Press **Reboot device**, just below. Network changes only take effect after
   a restart. The lamp comes back on your network, and its own `infinity-lamp`
   network disappears once it has joined.
4. From then on, reach it at **http://infinity-lamp.local** from any browser
   on your home network.

If it cannot find your network, it puts its own `infinity-lamp` network back up
so you are never locked out.

---

### 6. Things to try

- **Pick it up and turn it.** Effects such as *Rain*, *Gravity Fill* and
  *Spirit Level* follow which way is down.
- **Play some music.** Switch to *Spectrum*, *Bass Bloom* or *Sound Ripple*.
- **Give it a shake.** *Shake Sparkle* bursts when it is handled.
- **Turn on Auto-cycle** on the control page and let it work through the
  effects on its own.
- **Set it down and walk away.** After a few seconds without movement, the face
  resting on the table switches itself off to save power. Pick the lamp up and
  it comes straight back.

---

### Safety, briefly

- Indoor use only. Keep it dry.
- Do not cover the lamp or run it inside a cabinet or box.
- If you have fitted cells: do not drop it, crush it, or leave it in a hot car
  or in direct sun. Never fit a damaged or swollen cell, never mix old and new
  cells, and recycle old cells at a battery collection point rather than in the
  bin. If the lamp ever swells, gets hot, or smells odd, unplug it, move it
  somewhere non-flammable and contact me.
- Some effects flash or strobe. If you are sensitive to flashing light, avoid
  *Beat Strobe*, *Beat Pulse* and *Theatre Chase*.
- Not a toy. It is heavy and has rigid panels.

Full safety notes are in the User Guide.

---

### If something goes wrong

| Symptom | First thing to check |
|---|---|
| Nothing lights up | Is it a **PD** charger? Try the supplied one. Hold the button for 1 second. |
| Can't find `infinity-lamp` WiFi | It has already joined your home network. Try http://infinity-lamp.local |
| `infinity-lamp.local` doesn't load | Find its IP in your router's device list and use that instead |
| Some effects are missing | This lamp was built without that sensor. See the User Guide |

---

**Made by [MAKER NAME]**
Questions, spares or repairs: **[SUPPORT EMAIL]**
Full documentation: **[PROJECT URL]**

*Hand-built, one at a time. It is not a certified commercial product - please
read the safety notice in the User Guide.*

