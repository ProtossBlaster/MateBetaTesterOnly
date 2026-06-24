# Data collection consent — Mate BetaTester

By installing and using the **LeapMotor Mate — BetaTester** build you agree to the following.

## What is collected
- **All raw signals** your vehicle reports to the Leapmotor cloud, with timestamps, stored
  **locally** in the add-on/container database.
- The **logbook notes** you write.

## What leaves your device
- **Nothing automatically.** Data only leaves your device when **you** click *Export* and then
  **you** attach the resulting bundle to an issue.
- The exported bundle is **encrypted** with the maintainer's public key — only the maintainer's
  private key (kept off-repo, on the maintainer's machine) can open it.
- **GPS coordinates are stripped** from the export before it is encrypted.
- Anything you write in a logbook note, or any screenshot you attach, is your choice — please
  don't put personal data there.

## Why
To map REEV (range-extender) signals and behaviour so that **REEV support can be added to the
normal LeapMotor Mate**. This build is a temporary data-collection tool, not a finished product.

## Your control
- You can stop at any time: uninstall the add-on / remove the container.
- You can delete the captured data with the **Factory reset** in Settings.
- Don't want to take part? Simply use the official Mate instead:
  https://github.com/ProtossBlaster/leapmotor-mate

## Note on accuracy
Statistics, Costs, Trips and similar pages may be **inaccurate** in this build because REEV
behaviour is not yet integrated. This is expected — please do not report it.
