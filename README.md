# Anishkumar Patel QA CA Portfolio

![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Inter&size=32&pause=1000&color=61dafb&center=true&width=800&lines=Hi!+I%27m+Anishkumar+👋;QA+Automation+Engineer;Building+Reliable+Software;Let%27s+Automate+Together)

> My consolidated QA portfolio showcasing end‑to‑end testing: Web UI, API, Performance, Code Quality & Containerization.

<!-- GitHub stats -->

![Anish's GitHub stats](https://github-readme-stats.vercel.app/api?username=apatel2582&show_icons=true&theme=dark)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=apatel2582&layout=compact&theme=dark)

---

[![CI Status](https://img.shields.io/github/actions/workflow/status/apatel2582/apatel2582/build.yml)](https://github.com/apatel2582/apatel2582/actions) [![Quality Gate](https://sonarcloud.io/api/project_badges/measure?project=apatel2582_apatel2582&metric=alert_status)](https://sonarcloud.io/dashboard?id=apatel2582_apatel2582)

---

## Table of Contents

- [Anishkumar Patel QA CA Portfolio](#anishkumar-patel-qa-ca-portfolio)
  - [Table of Contents](#table-of-contents)
  - [About](#about)
  - [Modules](#modules)
  - [Prerequisites](#prerequisites)
  - [Quick Start](#quick-start)
  - [Running Tests](#running-tests)
    - [Web UI](#web-ui)
    - [API](#api)
    - [Performance](#performance)
  - [CI/CD](#cicd)
  - [Author \& Contact](#author--contact)

---

## About

A one‑stop showcase of my QA skillset—built with industry‑standard tools and best practices:

- **Java + Selenium (POM)**
- **RestAssured** for REST APIs
- **Apache JMeter** for load testing
- **GitHub Actions** CI
- **JaCoCo** & **SonarCloud** for code quality
- **Docker** & **Docker‑Compose** for containerized runs

---

## Modules

The main repo for my QA demonstration is `apatel2582/awesome-qa-portfolio`.
[Awesome QA Portfolio](https://github.com/apatel2582/awesome-qa-portfolio)
Each folder is a standalone framework. See its own `README.md` for details:

- **`web-ui-automation/`**  
  Page Object Model in Java + Maven, TestNG smoke tests, demo screenshots/GIFs.
- **`api-tests/`**  
  RestAssured suite (or Postman + Newman), 5+ endpoint tests.
- **`performance-tests/`**  
  JMeter plan (or Gatling scripts) with sample HTML reports.
- **`code-quality/`**  
  JaCoCo & SonarCloud setup, quality‑gate badge.
- **`container/`**  
  `Dockerfile` and `docker-compose.yml` to spin up tests & (optional) SUT.

---

## Prerequisites

- **Java 21** (JDK)
- **Maven 3.6+**
- **Gradle**
- **Docker 20.10+** & **Docker‑Compose 1.29+**
- **Git** (SSH key configured)
- _(Optional)_ **Node.js** & **Newman** for Postman collections

---

## Quick Start

```bash
# 1. Clone
git clone git@github.com:apatel2582/awesome-qa-portfolio.git
cd awesome-qa-portfolio

# 2. Run all UI & API tests
mvn clean test

# 3. Run performance tests (JMeter headless)
jmeter -n -t performance-tests/test-plan.jmx -l performance-tests/reports/results.jtl

# 4. Bring up containerized test runner
docker-compose up --build
```

---

## Running Tests

### Web UI

```bash
cd web-ui-automation
mvn test
```

### API

```bash
cd api-tests
# RestAssured:
mvn test
# Or Postman:
newman run collections/petstore.json
```

### Performance

```bash
cd performance-tests
jmeter -n -t test-plan.jmx -l reports/report.html
open reports/report.html
```

---

## CI/CD

All suites are wired into GitHub Actions (`.github/workflows/ci.yml`):

- **build** → compile + unit tests
- **ui-tests** → Selenium smoke tests
- **api-tests** → RestAssured/Newman runs
- **perf-tests** → JMeter headless
- **quality** → JaCoCo coverage + SonarCloud scan

---

## Author & Contact

**Anishkumar Pankajkumar Patel**

- [![GitHub](https://img.shields.io/badge/GitHub-%40apatel2582-181717?logo=github)](https://github.com/apatel2582)
- [![Email](https://img.shields.io/badge/Email-anishkumarp.ca@gmail.com-red?logo=gmail)](mailto:anishkumarp.ca@gmail.com)
- [![LinkedIn](https://img.shields.io/badge/LinkedIn-Anishkumar-blue?logo=linkedin)](https://www.linkedin.com/in/anishkumar-patel/)
