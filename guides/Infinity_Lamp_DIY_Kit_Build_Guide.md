# Tessera infinity lamp

## DIY Kit - Draft for feedback

Draft 0.1 - November 2026

---

## About this draft

**There is no DIY kit yet.** Finished lamps come first. A kit is planned as a
follow-up, and before I decide how to make it I would like to hear from the
people who might build one.

This document does two jobs:

- it describes what a kit **could** look like, and roughly how the build would
  go, so you can picture it,
- it asks the questions I need answered before deciding (*Your feedback*, at the
  end).

Nothing here is a promise of contents, price or date. Parts, steps and tiers will
change once I know what builders actually want. Where something is open it says
so.

---

## 1. What you would end up with

The same lamp as a finished one: a mirrored polyhedron with addressable LEDs
along every edge, controlled from any browser, with the same 34 effects, the same
sensors, the same optional USB-C power bank and the same free firmware updates.
Once it is built, the **User Guide** applies to it exactly as it does to a
finished lamp.

What changes is who does which part of the work.

---

## 2. How the lamp goes together

Whatever the kit tier, a lamp is built from the same five stages. Each one is a
candidate for doing yourself or having done for you.

| Stage | What it involves | Skill and tools |
|---|---|---|
| **A. Frame** | Printed struts (one per edge) glued into printed corner hubs, held square in a printed glue jig while the glue sets | Patience. Cyanoacrylate glue, the jig, a flat bench |
| **B. LEDs** | Cutting LED strip to edge length, laying it into each strut's channel, and soldering the strip ends together at each corner | Confident soldering of small pads. Soldering iron, the printed solder jig |
| **C. Electronics** | Fitting the controller board, power socket, power switch, button and power-bank bay into the base, and connecting the LED chain | Screwdriver. The board arrives assembled and tested in every tier |
| **D. Setting up** | Telling the lamp its shape and LED layout, then checking every edge with the built-in wiring check | A phone or laptop. No software to install |
| **E. Panels** | Cutting acrylic panels, applying mirror film, fitting them into the frame and clipping the covers on | Care and a dust-free room. Acrylic cutting tools, film application kit |

The controller board is always supplied **fully assembled, flashed and tested**.
It has fine-pitch surface-mount parts, and a bad joint on its power path is
invisible and only fails under load. That is not a step I can support at a
distance.

---

## 3. Possible kit tiers

These are the options I am weighing. The point of the feedback section is to
find out which of them anyone wants.

| | **Assembly kit** | **Builder's kit** | **Maker's pack** |
|---|---|---|---|
| Controller board, assembled and tested | Included | Included | Included |
| Power socket, switch, button, bay leads | Included, pre-wired | Included, pre-wired | Included, pre-wired |
| Frame parts | Printed, frame pre-glued | Printed, loose | Print them yourself from the published files |
| LED strip | Pre-cut and soldered into a finished chain | Cut to length, you solder the corners | You buy and cut it |
| Panels | Cut and mirrored | Cut and mirrored | You cut and mirror them, using the printed templates |
| Glue and solder jigs | Not needed | Printed jigs included | Print them yourself |
| Firmware | Installed and set up for your lamp | Installed and set up for your lamp | Installed. You enter your own shape and layout |
| Soldering | None | LED corners only | LED corners only |
| You need a 3D printer | No | No | Yes |

A **power bank is not included in any tier**. It is the only part with lithium
cells in it, and you buy it finished and certified (see section 5).

---

## 4. Draft build outline

This is the order the build would follow. Detailed steps, photos and part counts
will come once the kit contents are settled. Steps marked *(tier)* only apply to
kits where you do that stage yourself.

### 4.1 Check the kit

Unpack onto a soft cloth and check everything against the parts list before you
start. Leave the panels in their sleeves until the end: dust or a scratch on a
panel is permanent once the lamp is closed.

### 4.2 Build the frame *(tier)*

1. Dry-fit one strut into one hub to feel how firmly they seat.
2. Glue each strut into its hubs using the glue jig, which holds the joint at the
   right angle while the glue sets.
3. Build face by face, checking each face sits flat with no gap at any joint.

> **WARNING**
> Glue the frame **before** any panel is unpacked. Cyanoacrylate vapour fogs
> acrylic permanently, even without touching it.

### 4.3 Fit the LEDs *(tier)*

1. Lay each length of strip into its strut's channel, LEDs facing into the lamp,
   following the arrows printed on the strip and the wiring map.
2. Solder the strip ends together at each corner, using the solder jig to hold
   the two strips at the corner angle.
3. Do not kink the strip. A hard fold cracks its tracks and darkens everything
   after it.

### 4.4 Fit the electronics

1. Mount the controller board in the base.
2. Fit the power socket, the power switch and the button, and plug their leads
   into the board.
3. Connect the start of the LED chain to the board's LED terminal.
4. If your lamp has a power-bank bay, fit the bay lead. Do not fit a bank yet.

### 4.5 First power-on, with the lamp still open

1. Set the power switch to **OFF**, then plug in a **USB-C PD charger that offers
   20 V**. Set the switch to **ON**.
2. Join the lamp's own WiFi network, `infinity-lamp`, and open the control page.
3. Set brightness to about 30%, choose a white palette and *Solid / Gradient*,
   and look at every edge.

If anything gets warm, smells, or one LED lights very brightly while the rest stay
dark, switch off and contact me.

### 4.6 Set up and check the wiring

1. *(Maker's pack)* On the Advanced settings page, under **LED & shape config**,
   choose the shape and enter the LEDs per edge and the colour order.
2. Turn on **Wiring check**. It lights one segment at a time: amber, with a
   green first LED where the data enters and a white dot running the way the data
   flows. Compare each one with the **Unfold net** view.
3. If a segment runs the wrong way, tick **reversed** for it in the segment
   mapping. If two are swapped, exchange their edge numbers. Save.
4. Check the sensors: play music and watch the sound meters; tilt the lamp with
   *Gravity Fill* playing. Then sit the lamp upright and press **Calibrate
   level**.
5. On the Backup and provisioning panel, press **Use current settings as
   baseline**, so a future reset returns the lamp to your build.

### 4.7 Fit the panels *(tier)*

1. Clean hands or cotton gloves. Hold panels by their edges.
2. Lower each panel into its rebate square rather than sliding it in.
3. Clip the covers over the struts around it, working round the face.
4. Look through each panel at a light before moving on. Any dust you can see now
   will be in the tunnel for good.

### 4.8 Close up and run it in

1. Fit the base cover. Check no lead is pinched.
2. Run **Auto-cycle** for half an hour. It finds an intermittent connection while
   the tools are still out.
3. Export a backup from the Advanced settings page and keep the file.

From here the **User Guide** covers everything, including fitting a power bank.

---

## 5. The power bank

A kit lamp takes the same optional power bank as a finished one. It is not
included. It must have:

- a **USB-C PD output that offers [BANK PD VOLTAGE] V**,
- **20 W** or more,
- a **UKCA or CE mark**, bought from a proper retailer,
- a size that fits the bay: **[BAY DIMENSIONS]**.

One USB-C port is enough, and pass-through charging is not needed. The lamp
charges the bank while plugged in and switches to it when the mains goes. User
Guide section 13 has the detail.

---

## 6. Tools you would need

| Tool | Assembly kit | Builder's kit | Maker's pack |
|---|---|---|---|
| Small screwdriver | Yes | Yes | Yes |
| USB-C PD charger, 20 V, [CHARGER WATTAGE] W or more | Yes | Yes | Yes |
| Phone, tablet or laptop with a browser | Yes | Yes | Yes |
| Soldering iron, fine tip, and solder | - | Yes | Yes |
| Cyanoacrylate glue | - | Yes | Yes |
| Multimeter | - | Recommended | Recommended |
| 3D printer (PETG, matte black) | - | - | Yes |
| Acrylic cutting tools and mirror-film kit | - | - | Yes |

---

## 7. Your feedback

This is the part I need help with. Answer as many as you like, in any order, by
email to **[SUPPORT EMAIL]** or as an issue at
**[github.com/infinity-lamps/tessera/issues](https://github.com/infinity-lamps/tessera/issues)**
titled *Kit feedback*.

### About you

1. Have you built electronics or 3D-printed kits before? Roughly what?
2. Do you own a 3D printer? Which materials do you print?
3. How comfortable are you soldering small pads on LED strip: never tried,
   could learn, happy doing it?

### What the kit should include

4. Which tier in section 3 would you buy, if any? What would you change about it?
5. Would you rather the frame came pre-glued, or build it yourself?
6. Would you rather the panels came cut and mirrored, or cut and film them
   yourself? Mirror filming is the most skilled and least forgiving step.
7. Should a USB-C power bank be an option in the box, or are you happy to buy
   your own to the published specification?
8. Is a charger something you would want included?

### The lamp itself

9. Which shape, and roughly what size, would you most want to build?
10. Do the microphone and motion sensor matter to you, or would a cheaper kit
    without them be better?

### Instructions and support

11. How would you like the instructions: printed booklet, online guide, PDF,
    video, or a mix?
12. What would worry you most about building one?
13. What would you expect to pay for the tier you would choose?
14. Anything else you would want me to know?

Thank you. Every answer changes what the kit turns out to be.

---

**Made by Ryan in Scotland**

Questions and feedback: **[SUPPORT EMAIL]**

Guides, firmware and print files: **[infinity-lamps.github.io/tessera](https://infinity-lamps.github.io/tessera/)**

*Draft for feedback only. No kit is on sale, and the contents described here may
change.*
