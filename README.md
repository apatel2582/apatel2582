# Anishkumar Patel QA CA Portfolio

![Anishkumar Patel](https://avatars.githubusercontent.com/u/2582?s=200&v=4)

> My consolidated QA portfolio showcasing end‑to‑end testing: Web UI, API, Performance, Code Quality & Containerization.

---

[![CI Status](https://img.shields.io/github/actions/workflow/status/apatel2582/apatel2582/ci.yml)](https://github.com/apatel2582/apatel2582/actions)
[![Coverage](https://img.shields.io/codecov/c/github/apatel2582/apatel2582)](https://codecov.io/gh/apatel2582/apatel2582)
[![Quality Gate](https://sonarcloud.io/api/project_badges/measure?project=apatel2582_apatel2582&metric=alert_status)](https://sonarcloud.io/dashboard?id=apatel2582_apatel2582)

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
  - [Contributing](#contributing)
  - [License](#license)
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

- **Java 11+** (JDK)
- **Maven 3.6+** (or Gradle if preferred)
- **Docker 20.10+** & **Docker‑Compose 1.29+**
- **Git** (SSH key configured)
- _(Optional)_ **Node.js** & **Newman** for Postman collections

---

## Quick Start

```bash
# 1. Clone
git clone git@github.com:apatel2582/anishkumarpca.git
cd anishkumarpca

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

## Contributing

1. Fork the repo
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes & push (`git push origin feature/your-feature`)
4. Open a Pull Request, reference issues if any

Please abide by the [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) and run all tests locally before opening a PR.

---

## License

Distributed under the MIT License. See [`LICENSE`](LICENSE) for details.

---

## Author & Contact

**Anishkumar Pankajkumar Patel**

- GitHub: [@apatel2582](https://github.com/apatel2582)
- Email: anishkumarp.ca@gmail.com
- LinkedIn: [anishkumar‑patel](https://www.linkedin.com/in/anishkumar-patel/)
