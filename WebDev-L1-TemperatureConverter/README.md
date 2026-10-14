# Degree — Temperature Converter

**Internship:** Oasis Infobyte — Web Development & Designing  
**Level / Task:** Level 1, Task 3 — Temperature Converter Website  
**Folder:** `WebDev-L1-TemperatureConverter`

## Project overview

Degree is a responsive temperature conversion utility for Celsius, Fahrenheit, and Kelvin. It uses vanilla JavaScript to validate input, convert units, and explain invalid temperatures in a clear status message.

## Features

- Numeric temperature input with empty-value and numeric validation
- Separate selectors for the input unit and target/output unit
- Converts between Celsius (°C), Fahrenheit (°F), and Kelvin (K)
- Displays the requested converted value and its Celsius equivalent
- Converts when the input or unit selectors change, and also through a visible **Convert temperature** button
- Unit-swap control
- Quick examples for common reference temperatures
- Rejects values below absolute zero with a user-friendly error message
- Rounds displayed results to two decimal places and avoids negative zero
- Responsive layout, clear field labels, visible status text, keyboard focus styling, and reduced-motion support
- No external frameworks, libraries, or build tools

## Technologies

- **HTML5** — form controls, labels, and result area
- **CSS3** — layout, styling, responsive breakpoints, and illustration
- **Vanilla JavaScript** — conversion formulas, DOM event listeners, numeric checks, and result formatting

## Conversion approach

The script converts the input to Celsius first, then converts that Celsius value to the target unit:

- Fahrenheit to Celsius: `(°F - 32) × 5 / 9`
- Kelvin to Celsius: `K - 273.15`
- Celsius to Fahrenheit: `(°C × 9 / 5) + 32`
- Celsius to Kelvin: `°C + 273.15`

Absolute zero is `−273.15°C` (equivalent to `0 K` and `−459.67°F`). Values below this physical limit are rejected. Kelvin is displayed without a degree symbol.

## Run locally

1. Open this folder.
2. Open `index.html` in a modern browser.
3. Enter a value and choose the input/output units.
4. Try the example buttons and swap control; test empty input and a value below absolute zero.

## Screenshots and output evidence

Save genuine browser screenshots in `screenshots/` before submitting. Suggested filenames:

- `screenshots/converter-valid-result.png`
- `screenshots/converter-validation-error.png`
- `screenshots/converter-mobile.png`

Include a successful conversion and the below-absolute-zero validation state.

## Level 1, Task 3 — feature checklist

The boxes below reflect source-code inspection. An unchecked item is a known gap or a manual verification still to complete.

- [x] Numeric input field and checks for empty/non-finite input
- [x] Input unit selector with Celsius, Fahrenheit, and Kelvin
- [x] Separate output-unit selector
- [x] Visible **Convert temperature** submit button triggers the existing form validation and calculation
- [x] Result display with converted value and unit labels
- [x] User-friendly validation for values below absolute zero
- [x] Centred utility layout with labelled controls and result area
- [x] Visually inspect the generated desktop/mobile and valid/error screenshots; conversion results are automatically tested by the verification script
- [x] Generate genuine desktop/mobile, valid-result, and validation-error screenshots in `screenshots/`

## OIBSIP submission checklist

- [ ] Keep this folder name exactly `WebDev-L1-TemperatureConverter` inside the repository named `OIBSIP`.
- [ ] Commit the source, this README, and screenshots/output evidence to the public `OIBSIP` repository.
- [ ] Record an end-to-end demo. The first **2 seconds** must be a static title card showing **Shreya Seal**, **Web Development & Designing**, and **Temperature Converter Website**; then demonstrate valid conversion and validation.
- [ ] Post/link the demo on LinkedIn, tag Oasis Infobyte, and include `#oasisinfobyte` (a relevant tag such as `#webdevelopment` may also be used).
- [ ] Leave substantive comments on at least two other interns' demo videos.
- [ ] Submit the task form shared through the internship/orientation email and include the OIBSIP repository link.

## Test cases to demonstrate

| Input | From | To | Expected result |
|---:|---|---|---:|
| 0 | Celsius | Fahrenheit | 32°F |
| 100 | Celsius | Fahrenheit | 212°F |
| 32 | Fahrenheit | Celsius | 0°C |
| 273.15 | Kelvin | Celsius | 0°C |
| -300 | Celsius | Fahrenheit | Error: below absolute zero |
