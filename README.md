# MI Result Hub

Semester grade calculator for Math et Informatique (MI) students, L1 and L2.

## Features
- Academic year (2026/2027 to 2030/2031), level (L1, L2) and semester (S1 to S4) selection. Modules appear only after the level and semester are chosen.
- Official modules, coefficients, credits and evaluation types for S1, S2, S3 and S4 (see `ACADEMIC_DATA` in `index.html`).
- Grade fields shown per module according to its evaluation type (TD+TP+Exam, TD+Exam, TP+Exam, Exam only). Grades must be between 0 and 20.
- Enter key moves to the next field; after the last grade it focuses the calculate button.
- Result page / certificate with name, registration number, major, year, level, semester, average and status.
- A different sound for a passing and a failing result (local files in `assets/`).
- Arabic / English interface, matrix-themed dark design, visitor counter.

## Project structure
```
index.html        calculator (data, calculation and validation are inside)
Result.html       result page / certificate
assets/success.mp3
assets/fail.mp3
```

## Run locally
Open `index.html` in a browser, or serve the folder: `python3 -m http.server 8000` and visit http://localhost:8000.

## Notes
- Browsers may block sound that starts without a prior user interaction. In that case the sound starts on the first tap/click/key on the result page (no visible audio controls are added).
- The visitor counter uses https://abacus.jasoncameron.dev (namespace and key are constants at the top of the counter code in `index.html`).

## License
MIT (add a LICENSE file to the repository if you want it published with the code).
