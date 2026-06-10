# SignalForm Assembly Guide

**Estimated build time:** 3–4 hours  
**Skill level:** Intermediate — soldering required for the power button mod and DC power patch cable. Skip both if you want a no-solder build (see notes in each step).  
**Tools needed:** Soldering iron, crimping tool, hot glue gun, CA glue, 5-minute epoxy, clear silicone, M3 hex driver, wire stripper

---

## Bill of Materials

| Part | Source | Part # | Qty | Unit Price |
|------|--------|--------|-----|------------|
| Dayton Audio DMA105-8 4" Full-Range Driver 8Ω | Parts Express | 295-591 | 2 | $18.98 |
| Dayton Audio ND105-PR 4" Passive Radiator | Parts Express | 290-213 | 2 | $13.98 |
| Dayton Audio KABD-250 2×50W Amp Board (BT 5.0 aptX HD) | Parts Express | 325-107 | 1 | $63.98 |
| Dayton Audio KABD-SPF Function Cables | Parts Express | 325-117 | 1 | $11.29 |
| Dayton Audio LBB-5Sv2 5×18650 Battery Charger Board 21V | Parts Express | 325-210 | 1 | $31.98 |
| Dayton Audio LBB-5CL DC Charging + Power Cable Kit | Parts Express | 325-142 | 1 | $9.98 |
| 18650 3.7V Li-Ion Batteries | Amazon | — | 5 | ~$15 |
| 12mm Stainless Latching Push Button (prewired) | Amazon | Gebildet 3-pack | 1 | ~$4 |
| Panel-Mount USB-C Port (2-pin) | Amazon | ALMOCN 5-pack | 1 | ~$6 |
| M3 Heat Set Inserts | Amazon | — | 14 | ~$5 |
| M3 Screws (6mm + 10mm) | Hardware store | — | assorted | ~$3 |
| Female spade connectors (matching driver terminal size) | Hardware store | — | 4 | ~$2 |
| Polyfill acoustic stuffing | Craft/fabric store | — | small bag | ~$3 |
| 5-minute epoxy | Hardware store | — | 1 tube | ~$4 |
| Clear silicone sealant | Hardware store | — | 1 tube | ~$5 |
| CA glue (super glue) | Hardware store | — | 1 tube | ~$3 |
| Hot glue sticks | Hardware store | — | a few | ~$2 |

**Total: ~$160**

> **Note on the DMA105-8:** This driver has occasionally been back-ordered at Parts Express. The DMA105-4 (4Ω, part #295-349) is a compatible alternate — the KABD-250 handles both impedances.

---

## Printed Parts (from signalform.3mf)

- Left speaker enclosure body
- Right speaker enclosure body
- Left rear backplate
- Right rear backplate
- Center electronics bay
- Front grille (left)
- Front grille (right)
- Handle
- Feet (×4)
- Knob caps (×3 — volume, bass, treble)

All parts printed in **PETG**. See README for print settings.

---

## Step 1 — Install Heat Set Inserts

Do this first, while all parts are separate and easy to handle.

- Set your soldering iron to ~200–220°C
- Press inserts into the cover mounting holes on the center electronics bay
- Press inserts into the handle mounting point on the top of the electronics bay
- Let all inserts cool fully before moving on

The left and right speaker enclosure backplates are sealed with epoxy only — no heat set inserts.

---

## Step 2 — Install the Handle

The handle goes on before the chambers are sealed — you won't be able to reach the mounting point after.

- Apply a small amount of **5-minute epoxy** to the handle base where it contacts the enclosure
- Set the handle into position and fasten with M3 screws into the heat set inserts from Step 1
- Hold firm until epoxy sets (~5 minutes)
- Let cure fully before any stress on the handle

---

## Step 3 — Make the DC Power Patch Cable

The KABD-250 needs full power delivered through its 12–24V DC input port. The LBB-5CL cable kit includes two wires with the correct barrel connectors on each end — solder them together to create a short patch cable that bridges the LBB-5Sv2 battery board output to the KABD-250 DC input.

- Take the two included power wires from the LBB-5CL kit
- Solder + to + and − to − to create a single patch cable with a connector on each end
- Heat shrink or tape each joint
- Set aside — this connects in Step 11

> **No-solder option:** Skip this step and use the toggle switch and default power wiring that comes with the LBB-5CL kit. You'll skip Step 13 as well. The build works fine this way — you just won't have the latching push button or the dedicated DC patch.

---

## Step 4 — Install Passive Radiators

Passive radiators mount on the outer side faces of each speaker enclosure — no wiring, purely mechanical.

- Apply a thin continuous bead of **clear silicone** around the passive radiator mounting flange
- Set each radiator into its recess on the enclosure side panel
- Press firmly and let cure for 30 minutes minimum
- Silicone only — no epoxy. These need to flex.

---

## Step 5 — Crimp Spade Connectors onto Driver Wires

Before the drivers go in, prep their wires for clean connections to the amp board terminals.

- Strip ~6mm of insulation from each driver lead (+/−)
- Crimp a female spade connector onto each lead
- Tug each crimp firmly to confirm it won't pull off — a bad crimp here causes intermittent sound loss

---

## Step 6 — Install Full-Range Drivers

- Thread the driver wires through the wire pass-through hole into the electronics bay channel first, before seating the driver
- Apply a thin bead of **clear silicone** around the driver mounting flange
- Seat each DMA105-8 into its front baffle recess
- Secure with M3 screws into the printed mounting holes — snug but not over-torqued, you're threading into plastic
- Let silicone cure before the next step

---

## Step 7 — Seal the Wire Pass-Through

Once driver wires are routed through to the electronics bay, seal the pass-through hole completely with **hot glue**. This is an acoustic boundary — any air path between the speaker chamber and electronics bay will hurt bass performance.

Pack the hot glue flush and let it set fully before moving on.

---

## Step 8 — Test Before Sealing

**Do not seal the enclosures until you've confirmed both sides work.** This is the last point where fixing a wiring issue is easy.

- Temporarily connect the driver spade connectors to the KABD-250 output terminals (left and right)
- Install all five 18650 cells into the LBB-5Sv2 battery board (observe polarity marked on each slot)
- Connect the DC patch cable from Step 3 between the LBB-5Sv2 output and the KABD-250 12–24V DC input
- Power on and play audio through Bluetooth
- Confirm both drivers produce sound and passive radiators are moving
- Check for any rattle or buzz at moderate volume

Fix anything before proceeding.

---

## Step 9 — Stuff the Speaker Chambers

With drivers confirmed working:

- Pull apart a small amount of polyfill and loosely fill each speaker enclosure cavity — about 1/3 full
- Don't pack it tight. Loose fill damps internal resonance without restricting passive radiator movement.

---

## Step 10 — Seal the Backplates

This step is permanent. The left and right speaker chambers close with epoxy and silicone only — no screws, no inserts.

- Apply a continuous bead of **5-minute epoxy** around the full perimeter of each backplate
- Set the backplate onto the enclosure and apply light even pressure
- Once epoxy is set, run a second bead of **clear silicone** along the inside seam
- The combination creates an airtight acoustic seal — any gap kills bass output

Let cure fully (1 hour minimum) before handling.

---

## Step 11 — Wire the Electronics Bay

With both speaker chambers sealed and driver wires routed in:

- Connect driver spade connectors to KABD-250 Left and Right output terminals (observe +/− polarity)
- Plug KABD-SPF function cables into the board header — these run to the volume, bass, and treble knobs, no soldering required
- Connect the DC patch cable (Step 3) between the LBB-5Sv2 output and the KABD-250 12–24V DC input port
- Install all five 18650 cells into the LBB-5Sv2 battery board (observe polarity marked on each slot)
- Connect the USB-C panel mount port leads to the LBB-5CL charging cable input on the LBB-5Sv2

---

## Step 12 — Bluetooth Antenna

The KABD-250 includes a small external Bluetooth antenna on a short cable.

- Plug the antenna connector into the board's antenna port
- Position the antenna flat against the top interior surface of the electronics bay
- Secure with a small drop of **CA glue** — keep it away from the connector itself
- Good antenna placement = better Bluetooth range through the enclosure walls

---

## Step 13 — Install the Push Button

The KABD-250 / LBB-5CL kit includes a toggle switch with two wires and a connector. The 12mm latching push button replaces it for a cleaner look and feel.

- Cut the two wires on the included toggle switch, leaving enough length to work with
- Strip ~6mm of insulation from each cut end
- Solder each wire to the two terminals on the 12mm latching push button
- Heat shrink or tape each joint
- Thread the button through its 12mm panel hole from inside, secure with the locking nut from outside

> **No-solder option:** Skip the push button entirely. Install the included toggle switch through a panel hole instead. It functions identically — just a different look.

---

## Step 14 — Install the USB-C Port

- Press the panel-mount USB-C port into its recess
- Secure with the two small machine screws included with the port
- Confirm the leads are connected to the LBB-5CL charging input (Step 11)

---

## Step 15 — Install Knob Caps

- Press the three printed knob caps onto the KABD-SPF potentiometer shafts
- Friction fit — no glue needed

---

## Step 16 — Close the Electronics Bay

- Route all wiring cleanly — no wires pinched against edges or near moving parts
- Set the bay cover and fasten with M3 screws into the heat set inserts from Step 1
- Snug but not over-torqued

---

## Step 17 — Attach Feet and Grilles

- Apply a small drop of **CA glue** to each foot mounting point on the underside, press and hold 30 seconds
- Apply CA glue around the grille mounting perimeter on each speaker face, press grilles into place and hold 30 seconds

---

## First Power On

**LBB-5Sv2 first-use wake:** The battery board requires a one-time initialization on first use. Install all five 18650 cells, then apply power through the USB-C port (any 5V USB charger). This wakes the board's protection circuit. Without this step the board will not output power regardless of battery charge level.

1. With batteries installed, plug in via USB-C to wake the LBB-5Sv2
2. Once the board LED activates, unplug USB-C
3. Press the latching power button — it clicks and stays engaged
4. The KABD-250 LED illuminates; Bluetooth pairing mode activates automatically
5. Pair your device — search for "KABD" or the board's default name
6. Set all three knobs to center (12 o'clock) for flat response to start
7. Play something. Adjust to taste.

---

## Troubleshooting

**No sound from one side:** Check driver spade connector polarity at the KABD-250 terminals. Swap +/− if needed.

**Low volume / underpowered:** Confirm the DC patch cable is connected between the LBB-5CL and the KABD-250 12–24V DC input port. Running from the board's onboard power path alone limits output.

**Weak or boomy bass:** Check passive radiator silicone seal for gaps. Verify the wire pass-through is fully sealed with hot glue. Verify polyfill isn't packed too tightly.

**Board won't power from battery:** Verify all five 18650 cells are seated correctly in the LBB-5Sv2 with polarity matching the markings on each slot. If this is first use, the board may need to be woken — plug in via USB-C with batteries installed to initialize the protection circuit. Confirm the push button or toggle switch is fully engaged.

**Buzzing or rattle:** Check backplate epoxy seams for gaps. A small air leak produces audible resonance at volume.

**Poor Bluetooth range:** Check that the antenna is plugged in and positioned flat against the top interior of the electronics bay.

---

## Remixing

CC BY 4.0 — build it, sell it, modify it. Credit Eric Brunner / Printed Pulse.

If you improve something, open an Issue and show the build.
