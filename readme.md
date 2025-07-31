> ⚠️ This repository is based on the [cypress-heroes](https://github.com/cypress-io/cypress-heroes) project, with structure, organization, and automated test writing developed with a focus on QA practice and learning.

---

# 🦸‍♂️ Cypress Heroes - E2E Test Automation Project

A fully automated end-to-end testing project built with **Cypress**, focused on dynamic validations, conditional tests, and real-world user simulation for the **cy.heroes** application.

---

## 🧪 About the Project

This project simulates real interactions in a hero management app where users can **create, edit, delete, and interact with heroes**, applying solid E2E testing practices.

Covered flows include:
- Login and authentication
- Hero creation and editing
- Action buttons (like, hire, edit, delete)
- Field validation with valid and invalid inputs
- Conditional modal messages based on login state
- Dynamic data generation and randomization

---

## 🚀 Technologies Used

- [Cypress](https://www.cypress.io/) — Main E2E test framework
- [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [Chance.js](https://chancejs.com/) — Random data generation
- [Google Sheets](https://www.google.com/sheets/about/) — For test planning and documentation

---

## 🎯 Project Goals

- Practice real-world test automation with broad feature coverage
- Apply conditional validation logic (e.g., modal behavior changes with login state)
- Use dynamic/random data for realistic testing
- Showcase clear structure, technical know-how, and testing principles
- Present a portfolio-ready QA project to recruiters and tech teams

---

## 🧠 Key Features Tested

| Test Area       | Description |
|-----------------|-------------|
| 🔐 Login        | Valid login using fixture data |
| 🧾 Create Hero  | Fill out form using generated data |
| ✏️ Edit Hero    | Clear and update input values |
| 🗑️ Delete Hero  | Delete and confirm redirection to home |
| 🏠 Home Actions | Like and hire buttons with dynamic target selection |
| 📋 Conditional Tests | Modals behave differently for logged-in vs. guest users |

---

## 📁 Project Structure

```bash
cypress/
│
├── fixtures/
│   ├── example.json
│   └── userData.json          # Fixture data (user credentials, etc.)
│
├── screenshots/               # Visual evidence from test runs
│
├── support/
│   └── commands.js            # Custom Cypress commands (if needed)
│
└── tests/
    ├── e2e/
    │   ├── createHero.spec.js
    │   ├── editHero.spec.js
    │   ├── homeActionButtons.spec.js
    │   └── login.spec.js
    │
    └── pages/                 # Page Object files to organize test selectors
        ├── createHeroPage.js
        ├── editHeroPage.js
        └── homePage.js        
```

---

## 📈 Centralized Test Documentation

The full testing strategy is tracked and documented in a shared spreadsheet, covering:

- ✅ Test Cases
- 🐞 Bug Reports
- 💡 Improvement Suggestions
- 📋 Test Run Reports

📎 [Google Sheets - Full Documentation](https://docs.google.com/spreadsheets/d/1sYQRylVOZbIfz2e6ZqTkMWKqxa38D9BU/edit?gid=1153597396)

---

## 🖥️ How to Run Locally

### Prerequisites
- Node.js installed
- Cypress installed via `npm`

### Steps

```bash
# Clone the repository
git clone https://github.com/marcusphillipe/cypress-heroes.git
cd cypress-heroes

# Install dependencies
npm install

# Set up database
npm run setup

# Start server
npm run dev

# Open Cypress test runner
npx cypress open
```

Select one of the `*.spec.js` files and execute it through the Cypress UI.

---

## 👨‍💻 Author

Project developed for learning, professional growth, and showcasing QA automation skills.

**Marcus Phillipe**  
🔗 [LinkedIn](https://www.linkedin.com/in/marcusparamos/)  
📁 [GitHub Repo](https://github.com/marcusphillipe/cypress-heroes)

---

## 🎯 Final Notes

This project was built with a focus on real testing workflows, clean architecture, and dynamic validations.  
It represents a complete QA workflow, from test design and automation to documentation and execution — ideal for professional portfolios and real project simulation.