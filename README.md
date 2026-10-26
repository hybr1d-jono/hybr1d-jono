![QA banner v2](https://github.com/user-attachments/assets/7ad42b51-76d5-4940-bb3f-e4ca1681eca7)

<h2>"Tell me and I forget; teach me and I remember; involve me and I learn."</h2>

## About Me 👋

```python
class WhoAmI:
    user = 'Jonathan Flavell'
    current_work = 'Quality Assurance'
    experience = 'Over 10 years in Quality Assurance, from fintech payments to veterinary SaaS'
    hobbies = [
        'Travel',
        'Sport',
        'Nature Walks',
        'Finding Defects ;p',
    ]

    def get_city(self):
        return 'Auckland, New Zealand'

    def ambitions(self):
        return ['ScaleAutomation', 'LeadQuality', 'EvolveQAWithAI']
```

[![LinkedIn Badge](https://img.shields.io/badge/-Jonathan_Flavell-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/qajono/)](https://www.linkedin.com/in/qajono/) [![Hotmail Badge](https://img.shields.io/badge/-jflavell@hotmail.com-c14438?style=flat-square)](mailto:jflavell@hotmail.com)

## Why Am I Here 🏢

Times are changing, and I'm changing with them. I'm sharing my journey as I keep levelling up in Quality Assurance and Business Analysis, and showcasing some of the work I've delivered along the way.

## Featured Work 🚀

> Work delivered at my current role on a veterinary practice management SaaS platform. Described at a high level to respect confidentiality, so no internal code or ticket details are shared.

Samples of my work across business analysis and quality assurance: requirements discovery, product and process documentation, and runnable test code.

Most of my professional work lives in private company repos, so everything here is either recreated against a fictional demo app or sanitised to remove company code, names and data. The approach and reasoning are the real thing.

What's in here

Grouped from analysis and product thinking, through quality strategy, to hands-on testing.

1. Business Analysis & Product Thinking
Sample	Shows
Discovery: Invoice-Level Sales Tax Cap	Requirements discovery, decision logs, domain research, stakeholder facilitation
User Journey Template	Persona-driven journeys written from the user's point of view, doubling as a coverage tracker
FQI Metrics	Designing a quality metric and building repeatable reporting from source data
Retro Facilitation	Scrum master practice: turning team discussion into owned, measurable actions
2. Quality Strategy & Leadership
Sample	Shows
Deciding What to Automate	Risk-based prioritisation framework: WHAT, WHICH, WHERE
E2E Failure Triage	Root-cause analysis, separating environment issues from flaky tests from real bugs
Automation Champion Guide	Coaching manual testers into automation
3. Hands-on Testing & Engineering
Sample	Shows
Merge Request Write-ups	Real changes I merged: what the problem was, what I did, why it mattered
XSS Testing Guide	Security testing method for verifying XSS fixes
Playwright E2E tests	Page objects, stable locators, shared helpers, data-driven scenarios
Unit tests	Characterisation tests for tax logic, including edge cases

How it connects: the tax cap discovery defines the business rules, the user journey describes them from the customer's side, and the tests prove them.

Run it (under 5 minutes)

Needs Node 20+.

bash
git clone https://github.com/hybr1d-jono/ba-qa-portfolio.git
cd ba-qa-portfolio
npm install
npx playwright install chromium
npm test

npm test runs the unit tests, starts the demo app, and runs the Playwright suite against it. To poke at the app yourself, run npm run demo and open http://localhost:4173.

Project layout
demo-app/            Fictional "ClinicBill" invoice app the tests run against
  tax.js             Tax logic: per-line tax, optional invoice-level cap
tests/
  unit/              Node test runner, no browser needed
  e2e/
    pages/           Page objects
    helpers/         Shared helpers (e.g. a toast wait that won't flake)
    *.spec.ts        Playwright specs
docs/                Sanitised documentation samples
.github/workflows/   CI: runs everything on every push
Things worth looking at in the code
No force clicks, no sleeps. Every wait is an assertion on something real.
Stable locators only. Every element is found by data-testid.
The toast helper. The demo app's save takes 1.5 seconds on purpose. A 1 second wait would fail. This mirrors a real fix I made that stabilised five tests at once.
Scenarios as data. The tax cap tests loop over a scenario table that matches the discovery doc.

## Tech Skills 💻

**Testing:** Test planning, risk-based prioritisation, functional, regression, smoke and UAT testing, test case design, bug reporting and the bug life cycle
**Automation:** Playwright E2E, test data seeding, flaky test remediation, coverage tracking
**APIs & Data:** REST API testing, SQL
**Ways of Working:** Agile Scrum, shift-left testing, documentation
**Other:** AI-assisted QA, basic HTML and CSS

## Tools I Use 🧰

<p align="center">
  <img src="https://img.shields.io/badge/Playwright-000?style=for-the-badge&logo=playwright&logoColor=white" alt="Playwright">
  <img src="https://img.shields.io/badge/Jira-000?style=for-the-badge&logo=jira&logoColor=white" alt="Jira">
  <img src="https://img.shields.io/badge/Xray-000?style=for-the-badge" alt="Xray">
  <img src="https://img.shields.io/badge/Zephyr-000?style=for-the-badge" alt="Zephyr">
  <img src="https://img.shields.io/badge/Confluence-000?style=for-the-badge&logo=confluence&logoColor=white" alt="Confluence">
  <img src="https://img.shields.io/badge/MySQL-000?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL">
  <img src="https://img.shields.io/badge/React-000?style=for-the-badge&logo=react&logoColor=%2361DAFB" alt="React">
  <img src="https://img.shields.io/badge/Postman-000?style=for-the-badge&logo=postman&logoColor=white" alt="Postman">
  <img src="https://img.shields.io/badge/Insomnia-000?style=for-the-badge&logo=insomnia&logoColor=white" alt="Insomnia">
  <img src="https://img.shields.io/badge/GitLab-000?style=for-the-badge&logo=gitlab&logoColor=white" alt="GitLab">
  <img src="https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  <img src="https://img.shields.io/badge/TeamCity-000?style=for-the-badge&logo=teamcity&logoColor=white" alt="TeamCity">
  <img src="https://img.shields.io/badge/Sauce_Labs-000?style=for-the-badge&logo=saucelabs&logoColor=white" alt="Sauce Labs">
  <img src="https://img.shields.io/badge/AWS-000?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="AWS">
  <img src="https://img.shields.io/badge/Datadog-000?style=for-the-badge&logo=datadog&logoColor=white" alt="Datadog">
  <img src="https://img.shields.io/badge/Grafana-000?style=for-the-badge&logo=grafana&logoColor=white" alt="Grafana">
  <img src="https://img.shields.io/badge/Slack-000?style=for-the-badge&logo=slack&logoColor=white" alt="Slack">
  <img src="https://img.shields.io/badge/Visual_Studio-000?style=for-the-badge" alt="Visual Studio">
  <img src="https://img.shields.io/badge/Google_Chrome-000?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Google Chrome">
</p>

## Side Projects 🏗️

- **EPL Fantasy Site:** built with the help of GitHub Copilot
- **Club Sport Admin**

## Other Stuff

![Jono's GitHub stats](https://github-readme-stats.vercel.app/api?username=hybr1d-jono&show_icons=true&hide=[%22issues%22])

<!---
hybr1d-jono/hybr1d-jono is a special repository because its `README.md` (this file) appears on your GitHub profile.
--->
