# GTU BME Otto and Diesel cycle efficiency calculator

For GTU Basic Mechanical Engineering (3110006, BE01000081, BE01R00081). Unit 3, Heat Engines and IC Engines, is 20% of the official BE01000081 syllabus, and together with Unit 2 makes 42% of the theory paper. Otto and Diesel cycle efficiency (numerical plus P-V diagram) is one of the topics GTU Hero's BME guide flags. Compression ratio daalo, efficiency lo.

Live page: https://princeadvant.github.io/gtu-bme-otto-diesel-efficiency/

## Formulas

- Otto: η = 1 − 1 / r^(γ − 1)
- Diesel: η = 1 − (1 / r^(γ − 1)) × (ρ^γ − 1) / (γ (ρ − 1))
- r = compression ratio, ρ = cut-off ratio, γ = 1.4 for air

## Test

`node test.js` checks the formulas against hand-worked values and prints `All checks passed`.

## Tips

- For the same compression ratio, Otto efficiency is higher than Diesel. Diesel engines win because they run much higher r.
- As cut-off ratio ρ tends to 1, the Diesel formula tends to the Otto value. The test file checks this.
- Always draw the P-V diagram. The guide lists these as numerical plus diagram questions.

Old papers and repeat counts: [GTU Hero](https://gtuhero.com/blogs/gtu-bme-paper-previous-year-papers-pyq) (GTU Hero is my project).
