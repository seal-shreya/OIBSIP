# Degree — Temperature Converter

**Internship:** Oasis Infobyte — Web Development & Designing  
**Level / Task:** Level 1, Task 3 — Temperature Converter Website  
**Folder:** `WebDev-L1-TemperatureConverter`

## Project Overview

Degree is a responsive temperature conversion utility for Celsius, Fahrenheit, and Kelvin.

It uses HTML, CSS, and vanilla JavaScript to accept temperature values, convert between units, and display validation messages for invalid temperatures.

## Features

- Numeric temperature input
- Separate input-unit and output-unit selectors
- Conversion between Celsius (°C), Fahrenheit (°F), and Kelvin (K)
- Visible **Convert temperature** button
- Converted result with unit labels
- Input validation for empty or invalid values
- Validation for temperatures below absolute zero
- Unit-swap control
- Quick examples for common reference temperatures
- Results rounded to two decimal places
- Avoidance of negative-zero display
- Responsive layout and labelled controls
- Keyboard focus styling and reduced-motion support

## Technologies Used

- **HTML5** — form controls, labels, and result area
- **CSS3** — layout, styling, and responsive breakpoints
- **Vanilla JavaScript** — conversion formulas, validation, and result formatting

No external framework, library, or build tool is required.

## Conversion Formulas

The conversion process uses Celsius as an intermediate value.

- **Fahrenheit to Celsius:** `(°F - 32) × 5 / 9`
- **Kelvin to Celsius:** `K - 273.15`
- **Celsius to Fahrenheit:** `(°C × 9 / 5) + 32`
- **Celsius to Kelvin:** `°C + 273.15`

Absolute zero is:

- `-273.15°C`
- `-459.67°F`
- `0 K`

Temperatures below absolute zero should be rejected. Kelvin is displayed without a degree symbol.

## How to Run

1. Open the `WebDev-L1-TemperatureConverter` folder.
2. Open `index.html` in a modern web browser.
3. Enter a temperature.
4. Select the input and output units.
5. Press **Convert temperature**.
6. Test the unit-swap control, quick examples, empty input, and below-absolute-zero validation.

## Screenshots

The `screenshots/` folder contains the following output evidence:

- `screenshots/converter-desktop.png`
- `screenshots/converter-mobile.png`
- `screenshots/converter-valid-result.png`
- `screenshots/converter-validation-error.png`

Open the screenshots to review the layout and the displayed conversion or validation state.

## Level 1, Task 3 — Checklist

- [x] Numeric input field
- [x] Input-unit selector for Celsius, Fahrenheit, and Kelvin
- [x] Separate output-unit selector
- [x] Visible conversion button
- [x] Result display with converted value and unit labels
- [x] Validation handling implemented in the source
- [x] Responsive layout and labelled controls
- [x] Desktop, mobile, valid-result, and validation-error screenshots generated
- [ ] Test representative conversions and compare the results with the expected values below
- [ ] Confirm empty input and below-absolute-zero values display the correct validation message
- [ ] Inspect desktop and mobile screenshots for clipping, overlap, and overflow

## Suggested Test Cases

|   Input | Input Unit | Output Unit |  Expected Result |
| ------: | ---------- | ----------- | ---------------: |
|       0 | Celsius    | Fahrenheit  |             32°F |
|     100 | Celsius    | Fahrenheit  |            212°F |
|      32 | Fahrenheit | Celsius     |              0°C |
|  273.15 | Kelvin     | Celsius     |              0°C |
| -273.15 | Celsius    | Kelvin      |              0 K |
|    -300 | Celsius    | Fahrenheit  | Validation error |
|   Empty | Any        | Any         | Validation error |

Small rounding differences may occur for decimal values.

## OIBSIP Submission Checklist

- [x] Project folder follows the required naming convention
- [x] Source code, README, and screenshots committed to the repository
- [ ] Record an end-to-end demo video
- [ ] Include a static title card for the first **2 seconds** showing:
  - **Name:** Shreya Seal
  - **Track:** Web Development & Designing
  - **Task:** Temperature Converter Website
- [ ] Demonstrate a successful conversion and an invalid-temperature case
- [ ] Post the demo on LinkedIn, tag Oasis Infobyte, and include `#oasisinfobyte`
- [ ] Leave substantive comments on at least two other interns' demo videos
- [ ] Submit the task form and include the repository link
