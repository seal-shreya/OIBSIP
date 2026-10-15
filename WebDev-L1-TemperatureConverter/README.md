# Degree — Temperature Converter

**Internship:** Oasis Infobyte — Web Development & Designing
**Level / Task:** Level 1, Task 3 — Temperature Converter Website
**Folder:** `WebDev-L1-TemperatureConverter`

## Project Overview

Degree is a responsive temperature conversion utility for Celsius, Fahrenheit, and Kelvin. Built with HTML, CSS, and vanilla JavaScript, it validates user input, converts temperatures between units, and displays clear results and validation messages.

## Features

- Numeric temperature input with empty-value validation
- Separate selectors for input and output units
- Conversion between Celsius (°C), Fahrenheit (°F), and Kelvin (K)
- Converted temperature and Celsius-equivalent displays
- Manual conversion using the **Convert temperature** button
- Automatic clearing of stale results when input or units change
- Unit-swap control
- Quick examples for common reference temperatures
- Validation for temperatures below absolute zero
- Results rounded to two decimal places, with negative-zero display avoided
- Responsive layout, labelled controls, keyboard focus styling, and reduced-motion support
- No external frameworks, libraries, or build tools required to run the website

## Technologies

- **HTML5** — form controls, labels, and result area
- **CSS3** — layout, styling, responsive breakpoints, and illustration
- **Vanilla JavaScript** — conversion formulas, validation, event listeners, and result formatting

## Conversion Approach

The application converts the input temperature to Celsius first, then converts the Celsius value to the requested output unit.

- Fahrenheit to Celsius: `(°F - 32) × 5 / 9`
- Kelvin to Celsius: `K - 273.15`
- Celsius to Fahrenheit: `(°C × 9 / 5) + 32`
- Celsius to Kelvin: `°C + 273.15`

Absolute zero is `−273.15°C`, equivalent to `0 K` and `−459.67°F`. Values below absolute zero are rejected. Kelvin is displayed without a degree symbol.

## Run Locally

1. Open the `WebDev-L1-TemperatureConverter` folder.
2. Open `index.html` in a modern web browser.
3. Enter a temperature and select the input and output units.
4. Click **Convert temperature** to calculate the result.
5. Try the quick examples, unit-swap control, empty input, and below-absolute-zero validation.

No installation or build step is needed.

## Screenshots and Output Evidence

The `screenshots/` folder contains browser screenshots of the website and its output states:

- `screenshots/converter-desktop.png` — desktop layout
- `screenshots/converter-mobile.png` — mobile layout
- `screenshots/converter-valid-result.png` — successful conversion
- `screenshots/converter-validation-error.png` — below-absolute-zero validation

## Feature Checklist

- [x] Numeric input field and empty-input validation
- [x] Input and output unit selectors for Celsius, Fahrenheit, and Kelvin
- [x] Conversion button and result display
- [x] Conversion logic and below-absolute-zero validation
- [x] Unit-swap control and quick-example buttons
- [x] Desktop, mobile, successful-result, and validation-error screenshots available
- [x] Automated browser checks for representative conversions
- [x] Automated check for empty-input rejection
- [x] Automated check for below-absolute-zero validation
- [x] Automated check for the water-freezing example
- [x] Automated check for unit swapping
- [x] Mobile viewport check at 375px with no horizontal overflow detected
- [x] Manually inspect all screenshots for visual clipping, overlap, and presentation issues

## OIBSIP Submission Checklist

- [x] Project folder is named `WebDev-L1-TemperatureConverter`.
- [x] Source code, README, and screenshots are present locally.
- [x] End-to-end demo video recorded with a static title card for the first **2 seconds**, showing **Shreya Seal**, **Web Development & Designing**, and **Temperature Converter Website**.
- [x] Demo includes a successful conversion and validation demonstration.
- [x] Publish the demo on LinkedIn, tag Oasis Infobyte, and include `#oasisinfobyte`.
- [x] Leave substantive comments on at least two other interns' demo videos.
- [x] Submit the official internship task form and include the public OIBSIP repository link.
- [x] Commit and push the final README updates to the public repository.

## Test Cases

|  Input | From       | To         |                      Expected result |
| -----: | ---------- | ---------- | -----------------------------------: |
|      0 | Celsius    | Fahrenheit |                                 32°F |
|    100 | Celsius    | Fahrenheit |                                212°F |
|     32 | Fahrenheit | Celsius    |                                  0°C |
| 273.15 | Kelvin     | Celsius    |                                  0°C |
|   -300 | Celsius    | Fahrenheit | Below-absolute-zero validation error |
|  Empty | Any        | Any        | Input validation prevents submission |

**Verification note:** The representative conversion, validation, quick-example, unit-swap, and mobile-overflow checks passed in automated browser tests. Manual visual inspection and final submission steps remain outstanding.
