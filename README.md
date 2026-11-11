# rocket-a4-simulation

Flight simulation of Rocket A4 (Ad Astra UC3M, TEKNOFEST 2027): the OpenRocket model of the rocket and
the preliminary design spreadsheet.

An OpenRocket `.ork` file stores both the rocket and its simulations, so there is no separate results folder.

## Structure

```
openrocket/   the rocket's .ork file (the baseline, with its simulations inside)
motors/       thrust curves (.eng / .rse) for motors that do not ship with OpenRocket
model/        preliminary design spreadsheet (Excel)
```

## Rules

- **One person at a time edits the baseline.** `.ork` and `.xlsx` files cannot be merged: if two people
  change them in parallel, one of the two versions is lost. Agree in the team before touching them.
- **Studies go in branches** named `<name>-d<week>-<Description>` (e.g. `nacho-d3-FinSize`) and reach `main`
  through a pull request approved by the Team Lead. Nobody commits directly to `main`.
- **Milestones are tags** on `main`: `baseline-pdr`, `baseline-cdr`.

Tools: OpenRocket, RASAero II and OSCALC are installed by the team setup (`vehicle` profile).
Full workflow: [`WORKFLOW.md`](https://github.com/Ad-Astra-UC3M/onboarding/blob/main/WORKFLOW.md).
