# Mixi's Pokemon Tracker

**Version 1.0.0**  
A browser-based RNG tracking tool for **Pokémon FireRed / LeafGreen on Nintendo Switch 1 and Switch 2**, built around **Ten Lines** workflows.

This tracker is designed to help with shiny hunting and RNG tracking by keeping your **Hunting target**, your **Hitting results**, and your **Shiny History** organized in one place.

---

## What it does

- Parses Ten Lines results directly from pasted text
- Automatically detects whether a hunt is **Wild** or **Static**
- Tracks your:
  - Seed + ms
  - Continue Screen Frames
  - Level
  - Gender
  - Nature
  - Pokémon
  - ms Calibration
  - Advances Calibration
- Lets you mark whether an entry is:
  - **Hunting**
  - **Hitting**
- Shows a **Current Hunt Target** panel
- Keeps an **Active Hunt Log**
- Keeps a separate **Shiny History**
- Stores data locally in your browser using `localStorage`
- Displays shiny sprites for the current target

---

## Who this is for

This tool is for players using **Ten Lines** and related RNG workflows for:

- **Pokémon FireRed / LeafGreen**
- **Nintendo Switch 1**
- **Nintendo Switch 2**

If you are tracking shiny targets, calibrations, and what you are actually hitting, this tool is meant to make that process easier.

---

## How to use it

### 1. Paste a Ten Lines result
Paste a Ten Lines output line into the input box.

The tracker will automatically detect whether the result is:

- **Wild**
- **Static**

---

### 2. Choose whether the entry is Hunting or Hitting
Use:

- **Hunting** for your target
- **Hitting** for what you actually got

The tracker prevents duplicate Hunting targets in the Active Hunt Log.

**Note**: After "Clear form" or "Clear all", the site automatically switches to Hunting, and once a line is pasted and "Save entry" is hit, it automatically switches to Hitting to make it easier for the user

---

### 3. Enter calibrations
Fill in:

- **ms Calibration**
- **Advances Calibration**

You can also use **Use Last Calibration** to quickly reuse the last saved values.

---

### 4. Save the entry
Click **Save Entry** to add it to the tracker.

---

## Static hunts

For **Static** hunts, the tracker will ask you to choose:

- a **Static Category**
- a **Static Pokémon**

This is used so the tool can display the correct target sprite and track the correct Pokémon.

Current Static categories include:

- Starters
- Fossils
- Gifts
- Game Corner
- Stationary
- Legends
- Events
- Roamers

---

## Buttons explained

### Save Entry
Parses the pasted Ten Lines result and saves it as either Hunting or Hitting.

### Use Last Calibration
Loads the most recently saved:

- ms Calibration
- Advances Calibration

### Redo Hunt
Clears the current Ten Lines entry and removes the **Hitting** rows under the current **Hunting** target, while keeping that Hunting target in place.

### Clear Form
Clears the current input fields, but does not wipe your logs.

### Clear All
Clears the current entry and the **Active Hunt Log**, but keeps **Shiny History**.

### Did It Shine?
Saves the current hunt target into **Shiny History**, asks for final calibrations, stores the number of attempts, and resets the Active Hunt Log for the next hunt.

---

## Data storage

This tracker stores your data using your browser’s **localStorage**.

That means:

- your data stays on your device/browser
- refreshing the page does **not** erase your logs
- switching browsers or devices will **not** carry the data over automatically
- clearing browser site data may erase saved tracker data

---

## Export / Import

### Active Hunt Log
You can export the Active Hunt Log as JSON.

### Shiny History
You can:

- export Shiny History as JSON
- import Shiny History from JSON

This is useful for backups or moving your Shiny History to another device/browser.

---

## Notes

- The tracker is built around the format used by **Ten Lines**
- Shiny sprites require an internet connection
- Static Pokémon selection currently depends on the user choosing the correct category and Pokémon
- This is the **first public release**, so community feedback is welcome

---

## Known limitations

- Static hunts currently rely on manual category/Pokémon selection
- Some edge-case species names or unusual output formats may need future adjustments
- The tracker is designed specifically around this RNG workflow and may not fit every possible use case

---

## Bug reports / feedback

If you find a bug or something behaves strangely, please open an issue and include:

- what you pasted into the tracker
- whether it was Wild or Static
- what you expected to happen
- what actually happened
- your browser/device if relevant

---

## Credits

Built by **Mixi**.

Created for the Pokémon RNG community with a focus on making shiny tracking cleaner, easier, and more organized.
