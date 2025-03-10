

# Playwright with Typescript - Cucumber - BDD

Learning automated testing using Cucumber and BDD.


# Project Structure Diagram

playwright-cucumber-bdd-typescript-main/
├── node_modules/
├── src/
│   ├── hooks/
│   │   └── hooks.ts
│   ├── helper/
│   │   └── report.ts
│   ├── test/
│   │   ├── features/
│   │   │   └── login.feature
│   │   ├── steps/
│   │   │   └── loginSteps.ts
│   │   └── test-results/
│   └── types/
│       └── multiple-cucumber-html-reporter.d.ts
├── .eslintrc.json
├── .prettierignore
├── .prettierrc.json
├── package.json
├── tsconfig.json
└── README.md

# Explanation
node_modules/: Contains all the npm packages installed for the project.
src/: The source directory for the project.
hooks/: Contains hook files for setting up and tearing down tests.
hooks.ts: Example hook file.
helper/: Contains helper files for the project.
report.ts: Example helper file for generating reports.
test/: Contains test-related files.
features/: Contains feature files written in Gherkin syntax.
login.feature: Example feature file.
steps/: Contains step definition files.
loginSteps.ts: Example step definition file.
test-results/: Directory to store test results.
types/: Contains custom type declaration files.
multiple-cucumber-html-reporter.d.ts: Type declaration for the multiple-cucumber-html-reporter module.
.eslintrc.json: ESLint configuration file.
.prettierignore: Prettier ignore file.
.prettierrc.json: Prettier configuration file.
package.json: Contains project metadata and dependencies.
tsconfig.json: TypeScript configuration file.






## Tutorials

- [Playwright Cucumber (BDD) - Typescript](https://www.udemy.com/course/playwright-cucumber-bdd-typescript)
- [Automated Software Testing with Playwright](https://www.udemy.com/course/automated-software-testing-with-playwright)


## Installation

1. **Install Playwright**:
   - Open VS Code.
   - Press <kbd>CTRL</kbd> + <kbd>SHIFT</kbd> + <kbd>P</kbd> to open the command palette.
   - Type `Install Playwright` and select it.
   - Click `OK` to install the required browsers.

2. **Install Cucumber plugin**:
   - Install the Cucumber plugin for VS Code from the extensions marketplace.

3. **Install dependencies**:
   - Open a terminal in your project directory and run the following commands:
     ```sh
     npm install @cucumber/cucumber --save-dev
     npm install ts-node --save-dev
     npm install fs-extra --save-dev
     npm install multiple-cucumber-html-reporter --save-dev
     ```

4. **Create necessary folders**:
   - Create the following folders in your project:
     ```
     src/test/features
     src/test/steps
     src/hooks
     src/helper
     ```
. **Install ESLint**:
   - Run the following command to install ESLint:
     ```sh
     npm install eslint --save-dev
     ```
   - Initialize ESLint configuration:
     ```sh
     npm init @eslint/config
     ```

6. **Configure ESLint and Prettier**:
   - Add Prettier to your ESLint configuration in `.eslintrc.json`:
     ```json
     "extends": [
       "eslint:recommended",
       "plugin:@typescript-eslint/recommended",
       "prettier"
     ],
     ```
   - Install Prettier:
     ```sh
     npm install --save-dev --save-exact prettier
     ```
   - Create a `.prettierignore` file with the following content:
     ```
     [package-lock.json](http://_vscodecontentref_/1)
     [README.md](http://_vscodecontentref_/2)
     ```
   - Create a `.prettierrc.json` file with the following content:
     ```json
     {
       "singleQuote": true
     }
     ```
   - Run Prettier to format your code:
     ```sh
     npx prettier --write .
     ```
   - Link Prettier with ESLint:
     ```sh
     npm install --save-dev eslint-config-prettier
     ```