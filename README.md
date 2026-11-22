# Medi_Calc
MediCalc is a browser-based clinical calculator platform featuring 15 health-related calculators.
MediCalc is a browser-based collection of clinical and health-related calculators. It brings common calculations into one searchable interface and presents results with formulas, plain-language explanations, limitations, and general advice.
What it includes
The current version contains 15 calculators and tools, grouped into six categories:
- Body and nutrition: Body Mass Index (BMI), Body Surface Area (BSA), Basal Metabolic Rate and estimated daily energy (BMR), Ideal Body Weight (IBW), and Waist-to-Hip Ratio (WHR).
- Heart and blood pressure: Mean Arterial Pressure (MAP), Corrected QT (QTc), and CHA₂DS₂-VASc.
- Kidney and blood tests: Estimated Glomerular Filtration Rate (eGFR), Creatinine Clearance (Cockcroft–Gault), corrected calcium, and anion gap.
- Diabetes: HbA1c and estimated average glucose.
- Pregnancy: Estimated due date based on the last menstrual period.
- Handy tools: Unit converter for selected weight, height, laboratory, and temperature units.
Main features
- Search calculators by name or topic.
- Enter values using labelled fields and displayed units/ranges.
- View calculated results, categories, formulas, quick-check examples, and stated limitations.
- Read result-related advice labelled in the interface as WHO-based guidance or general clinical guidance.
- View the most recent 30 results stored in the current browser.
- Copy a result summary.
- Print a result or use the browser's Save as PDF option.
- Switch between light and dark themes.
- Increase text size.
- Use the help window to understand the calculators and available features.
Technology
- HTML
- CSS
- Vanilla JavaScript
- Browser Local Storage for result history and text-size preference
- Google Fonts for typography when an internet connection is available
The submitted implementation is a single HTML file with embedded CSS and JavaScript. It does not require a server, database, account, API key, or build process for its core calculations.
How to run
1. Save the supplied source code as index.html.
2. Open the file in a modern web browser, or open the project folder in Visual Studio Code and run it with the Live Server extension.
3. Choose a calculator from the home screen or search by name/topic.
4. Enter the requested information and select Calculate.
5. Review the result, formula, advice, and limitations together.
A local development server is recommended for consistent browser behaviour. An internet connection is only needed for externally hosted fonts; the calculator logic itself runs in the browser.
Data and privacy
In the supplied version, the calculation and result display happen in the browser. The application does not implement user accounts or a project backend. It stores up to 30 recent result summaries and the text-size preference in the browser's Local Storage on that device. Clearing browser site data may remove these records. Do not use a shared or public device for sensitive information.

The page loads fonts from Google Fonts when available, which is an external network request. The current source does not send calculation results to a MediCalc server.
Important limitations
MediCalc is an educational and clinical-support prototype. It is not a diagnostic system and does not replace professional judgement, patient assessment, laboratory interpretation, or local clinical protocols.

Each calculator has its own intended population, assumptions, input requirements, and limitations. For example, some calculations are intended for adults, some assume stable kidney function, and some results need confirmation or interpretation alongside other clinical information. Read the limitations shown with each calculator before interpreting a result.

The interface labels some advice as WHO-based and other advice as general clinical guidance. These labels do not mean that the complete application has been clinically validated, certified, or approved by WHO or another medical authority.

Before real clinical deployment, all formulas, cut-offs, units, wording, and advice should be independently checked by qualified clinicians and compared with current local guidelines. Do not use MediCalc alone to diagnose, prescribe, change a medicine dose, or make an urgent treatment decision.
Suggested next improvements
- Add direct source references and publication/version dates for every clinical formula and recommendation.
- Arrange independent clinical review and documented verification tests for every calculator.
- Add clearer input validation and boundary-case tests.
- Improve accessibility testing with keyboard-only and screen-reader use.
- Add a carefully designed export format that avoids exposing sensitive information.
- Consider localization only after clinical translations have been reviewed by qualified people.
