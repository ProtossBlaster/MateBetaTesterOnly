# LeapMotor Mate — BetaTester

🔬 **Data-collection beta for building REEV (range-extender) support.** This is not the normal
Mate — install the official one if you just want to use Mate:
https://github.com/ProtossBlaster/leapmotor-mate

## ⚠️ Important
- **Statistics, Costs, Trips can be SKEWED** on a REEV here — REEV behaviour isn't integrated
  yet. This is expected. **Do NOT open issues about inconsistent data.**
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
