# LeapMotor Mate — BetaTester 🔬

Research build: the same Mate as the official one, plus full raw-signal capture, the logbook and
the encrypted export. See **DOCS.md** for the full guide and the
[repository README](https://github.com/ProtossBlaster/MateBetaTesterOnly).

✅ **REEV support is in the official build since 4.7.0.** This channel stays open for now, for the
testers who have not moved across yet — moving across is a backup and a restore, in that order:
[how to do it](https://github.com/ProtossBlaster/leapmotor-mate/blob/main/docs/BETA-TO-OFFICIAL.md).

⚠️ **Something that looks broken is worth an issue**: a refuel counted three times, a duplicate
row, a value that cannot be true. Use a Leapmotor account that your normal Mate isn't using at the
same time.

## Updating to Mate 4

Update an existing numbered BetaTester add-on (currently 3.19.2) normally. The `leapmotor_mate_beta` slug,
configuration, account and persistent `/data` stay in place; no extra setup,
certificate upload, export/import or migration command is needed. REEV and
mixed-model accounts that cannot qualify for the independent API automatically
keep the legacy compatibility backend. Signal collection and consent remain as
before.

Historical installs still reporting literal `beta` may have an update-dialog
version-ordering limitation. Supervisor supports an in-place update, but no
zero-extra-action migration has been verified for that historical UI path.
A reinstall or database export/restore is not inherently required.
