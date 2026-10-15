# RX3 Mod Ventotto

A mod for the **Pioneer XDJ-RX3** (firmware 1.20), plus **XDJ-RX3 Toolkit**, a Mac app that prepares the USB stick.

The mod runs **in RAM only**: it starts from the USB stick and never writes to the deck's system.
Switch the RX3 off and everything is back to stock.

> Personal, unofficial project, not affiliated with Pioneer DJ / AlphaTheta.

**Status:** everything below has been tested on a real XDJ-RX3, except two items still being
tested: **automatic app updates** and **"Make stems" in the Mac app**. Features marked **BETA**
are switched off by default.

---

## 🎛️ Stems

| Feature | On the deck |
|---|---|
| **4-part stems** | Every track can be split into **VOCALS, HARMONY, BASS and DRUMS**. The stems are made on the Mac and played on the deck. |
| **SLIP LOOP pads 1-4** | Switch VOCALS, HARMONY, BASS and DRUMS on and off. |
| **SLIP LOOP pads 5-8** | **Echo Out** of the part above: the part drops out and its echo keeps going, in time with the track. |
| **ISOLATOR ↔ STEMS** | **SHIFT + CUE** on a channel turns its HI / MID / LOW knobs into stem volumes (HI = vocals, MID = harmony, LOW = bass + drums). Press again to go back. One channel can be on STEMS while the other stays on ISOLATOR. |
| **STEMS panel on the screen** | One control per part, with its name and colour, and a level you can slide. |
| **Colour stems waveform** | The main waveform is drawn in the parts' colours, so you see which part is playing. It follows the knobs as you turn them. |
| **Fast stems loading** | Stems start playing right away; the rest of the file loads in the background while the track plays. |
| **MAKE STEMS from the deck** | On a track without stems, tap **MAKE STEMS**: the Mac (connected to the rear USB port) splits it and the deck loads the stems by itself when they are ready. |

## 🥁 Roll and effects

| Feature | On the deck |
|---|---|
| **ROLL on the touch screen** | The ROLL tab shows a row of squares from **1/1 to 1/32**. Tap and slide: the snare roll locks to the beat grid, wherever you start. |
| **HOLD** | Keeps the roll going without holding your finger on the screen. |
| **Roll filter** | While holding, swipe **up** for a high-pass, **down** for a low-pass. |
| **Roll volume** | With the AUX selector on **PORTABLE**, the **AUX LEVEL** knob sets the roll volume (LINE stays a normal input). |
| **BEAT FX on LOW / MID / HIGH** | In the FX tab, choose which bands the Beat FX works on: just the lows, the mids, the highs, or any mix. The rest stays clean. |
| **Sampler** | **RELEASE FX** (SHIFT + SLIP LOOP): 8 sample pads per deck (one shot, hold, loop, latch). The FX tab has a **SAMPLE VOLUME** slider. |

## 🔁 Performance

| Feature | On the deck |
|---|---|
| **Instant loops from CALL** | With no loop running, **CALL ◀** sets a **4-beat** loop and **CALL ▶** an **8-beat** loop. |
| **Custom BEAT JUMP** | BEAT JUMP and BEAT JUMP 2: 16 pads, each with its own jump (from ½ to 64 beats, forward or back), with the number shown on the pad. The pad lights turn off when the jump would leave the track. |
| **KEY SHIFT** | KEY panel: **-12 to +12 semitones** per deck, with no clicks when you engage it or go back to 0. |
| **Key Sync** | **SHIFT + BEAT SYNC** takes the deck to the key of the MASTER deck. BEAT SYNC on its own stays the normal sync. |
| **Key Match** | Harmonic suggestions in BROWSE: compatible keys are marked next to the tracks. |

## 🎨 Screen

| Feature | On the deck |
|---|---|
| **LIGHT theme** | White screen with dark text and a white waveform. Switch it in **Utility → DISPLAY MODE** or with **SHIFT + SHORTCUT**. |
| **Pioneer-style layout** | New panels, tabs and buttons drawn to match the native look, in both dark and light. |
| **ROLL and FX tabs** | They replace STATUS and BEAT FX on the touch screen. |
| **Asshole mode** | Tap the eye next to a deck's title to hide or show the track name. |
| **Custom logo** | Your own logo on the main screen. |
| **Loading notice** | The deck shows a message while the mod starts. |

## 🔍 Browse

| Feature | On the deck |
|---|---|
| **Accent-free SEARCH** | Type "cafe" and it finds "Café". |

## 🛡️ Reliability

| Feature | |
|---|---|
| **RAM only** | Nothing is written to the deck's system. Switch it off and it is back to stock. |
| **Safe start** | Hold **SHIFT** while inserting the USB stick to start without the mod. |
| **No restart on re-insert** | Pulling the stick out and putting it back does not restart the deck if the same mod is already running. |
| **Gentle on the USB stick** | During a set the mod keeps its log in memory and writes nothing to the stick. |
| **Guarded firmware hooks** | Every change checks the firmware first; if anything differs, that feature stays stock. |

---

## 📲 Mac app (XDJ-RX3 Toolkit)

| Feature | |
|---|---|
| **Install the mod** | Writes the mod to the USB stick in one click. |
| **Make stems** *(being tested)* | One button: reads the stick's rekordbox export, installs the separation engine the first time, and makes 4-part stems for the chosen playlist directly on the stick. Advanced options are tucked away. |
| **Stems on the Mac GPU** | The separation runs on the Mac (the deck does not have the power to do it). |
| **Stems from the deck** | Starts the link with the deck over the rear USB cable, for MAKE STEMS. |
| **Samples, Beat Jump, Roll** | Pages to set up sample banks, beat-jump pads and the roll. |
| **Look** | Light/dark theme and logo. |
| **Playlist reorder** | Change the playlist order; the deck shows the new order in BROWSE. |
| **Old mod warning** | Tells you when the stick carries an older mod than the app. |
| **Automatic updates** *(being tested)* | Tells you when a new version is out; **Update now** downloads it, replaces the app and reopens it. |

---

## 💾 BETA: mix without the USB stick

Pull the USB stick out (or press USB STOP) and the **MASTER track keeps playing** from the deck's memory (up to 14 MB).

- Off by default: switch it on in the app, **Look → BETA · Track in memory**.
- Known issues: the volume drops, the stick still shows in the settings, the USB STOP light blinks.
- Always press **USB STOP** before pulling the stick out.

---

## Safety

- Nothing is written to the deck's system: switch it off and it is back to stock.
- To start without the mod: hold **SHIFT** while you insert the USB stick.
- Always press **USB STOP** before pulling the USB stick out.
- Use an **exFAT** USB stick (MBR partition scheme).
