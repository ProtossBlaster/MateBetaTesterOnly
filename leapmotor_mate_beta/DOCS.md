# LeapMotor Mate — BetaTester

🔬 **Research build: the normal Mate plus full raw-signal capture, the logbook and the encrypted
export.** REEV support itself shipped in the official build with **4.7.0**:
https://github.com/ProtossBlaster/leapmotor-mate

## ⚠️ Important
- **This channel stays open for now** and keeps receiving every release, for the testers who have
  not moved across yet. Moving across is a backup and a restore, in that order: https://github.com/ProtossBlaster/leapmotor-mate/blob/main/docs/BETA-TO-OFFICIAL.md
- **The pages here are the official ones**, so the REEV figures match. One figure is still only
  here: the ⚡ electric rate of a generator drive (`reev_elec_kwh_100km`), which has never been
  held against a dashboard.
- **Something that looks BROKEN is worth reporting**: one refuel counted three times, a duplicate
  trip, a value that cannot be true.
- This build **logs all raw vehicle signals** locally. Nothing leaves your device until **you**
  export an **encrypted** bundle and attach it to an issue (GPS is stripped).
- **Use a Leapmotor account NOT used by your normal Mate at the same time** — two instances on
  one account evict each other's session.

## Setup
1. Open the add-on. A one-time consent screen explains the data collection — accept to continue.
2. Complete the wizard with a dedicated Leapmotor account (email / password / PIN), and pick your
   REEV variant.

## How to help
1. Drive / charge / refuel normally — signals are captured automatically.
2. On the **REEV** page, add **logbook notes** for notable events (e.g. *engine started to charge
   while driving*, *refueled to 100%*).
3. Take **official-app screenshots** (fuel level, fuel/EV/combined range, consumption, EV/fuel split).
4. **Export the encrypted bundle** (REEV page → *Export encrypted data bundle*).
5. Open an issue on the repo with the **bundle + screenshots** + a short description.

## Updating
The beta is a rolling image — to update, open the add-on and click **Rebuild**.

## Stopping / removing your data
Uninstall the add-on, or use **Factory reset** in Settings to wipe the captured data.
