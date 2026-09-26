# LeapMotor Mate — BetaTester 🔬

Data-collection beta for building **REEV (range-extender)** support. See **DOCS.md** for the
full guide and the [repository README](https://github.com/ProtossBlaster/MateBetaTesterOnly).

⚠️ Stats/Costs/Trips can be skewed here (REEV not integrated yet) — a number that just looks off
needs no issue. **Something that looks broken does**: a refuel counted three times, a duplicate
row, a value that cannot be true. Use a Leapmotor account that your normal Mate isn't using at the
same time.

## Updating to Mate 4

Update the existing BetaTester add-on normally. The `leapmotor_mate_beta` slug,
configuration, account and persistent `/data` stay in place; no extra setup,
certificate upload, export/import or migration command is needed. REEV and
mixed-model accounts that cannot qualify for the independent API automatically
keep the legacy compatibility backend. Signal collection and consent remain as
before; this does not change the limits on REEV statistics.
