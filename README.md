# 🔬 LeapMotor Mate — BetaTester (REEV data collection)

> **This is NOT the normal Mate.** It is a **beta-tester build whose only job is to collect data**
> so we can add **REEV (range-extender) support** to LeapMotor Mate. If you just want to use Mate,
> install the official one: **https://github.com/ProtossBlaster/leapmotor-mate**

---

## ⚠️ Read this first

- **The data on the pages can be WRONG.** Statistics, Costs, Trips, efficiency and similar pages
  may be **skewed / inconsistent** on a REEV — because REEV behaviour (e.g. the petrol engine
  charging the battery while you drive) is **not yet integrated**. That is expected.
- **🚫 Do NOT open issues about inconsistent / wrong data.** Those are known and are exactly what
  this beta exists to fix. Such issues will be closed.
- **This build logs ALL of your vehicle's raw signals** locally, so we can decode the REEV
  signals. Nothing is sent anywhere automatically — **you** choose when to export and send.
- **Use a Leapmotor account that your normal Mate is NOT using at the same time.** Two Mate
  instances on one account fight over the session ("Not authorised" / missing data).

By installing and using this build you agree to take part in this data collection. See
[CONSENT.md](CONSENT.md). A one-time consent screen also appears on first launch.

---

## What it does

1. **Captures every raw signal** the car reports, with timestamps (a full history, delta-logged).
2. **Logbook** — you add short timestamped notes for anything notable, e.g.
   *"engine started to charge while driving"*, *"refueled to 100%"*, *"switched to fuel mode"*.
3. **Encrypted export** — one click produces a bundle that is **encrypted so only the maintainer
   can open it** (your GPS is stripped out). You attach it to an issue here.

Pairing the raw signals with your logbook + official-app screenshots is how we map the REEV
signals correctly and then ship real REEV support in the normal Mate.

---

## Install

### Home Assistant add-on
1. Settings → Add-ons → Add-on Store → ⋮ → **Repositories**.
2. Add: `https://github.com/ProtossBlaster/MateBetaTesterOnly`
3. Install **LeapMotor Mate — BetaTester**, then open it.
4. **To update:** in the Add-on **Store**, open the top-right **⋮** menu → **Check for updates**; Home Assistant then offers the new version → open **LeapMotor Mate — BetaTester** and click **Update** (the beta image is a rolling tag, so HA only surfaces the update after that manual check).

### Docker
```bash
docker run -d --name mate-beta -p 4000:4000 -v mate-beta-data:/data \
  ghcr.io/protossblaster/leapmotor-mate:beta
```
(Docker Hub mirror: `protossblaster/leapmotor-mate:beta`.) Watchtower will keep `:beta` updated.

---

## How to help (the useful loop)

1. Drive / charge / refuel as usual. The build keeps capturing signals.
2. Whenever something notable happens, **add a logbook note** on the **REEV** page.
3. Take **screenshots of the official Leapmotor app** (fuel level, fuel/EV/combined range,
   consumption, the EV/fuel split) around the same time.
4. **Export the encrypted bundle** (REEV page → *Export encrypted data bundle*).
5. **Open an issue here** using the BetaTester template, attach the **bundle + your screenshots**,
   and describe what you did.

Thank you — this is exactly what makes real REEV support possible. 🙏

---

Built from the same source as the official Mate (`MATE_RESEARCH=1`). Mapping work draws on
[kerniger/leapmotor-ha#46](https://github.com/kerniger/leapmotor-ha/issues/46).
