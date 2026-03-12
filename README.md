# SauceDemo Automation Testing Framework

## Project Overview

This project is a **web automation testing framework** built for the demo e-commerce website SauceDemo. The framework follows industry-standard automation practices such as **Page Object Model (POM)**, modular architecture, and automated HTML reporting.

The objective of this project is to demonstrate how a professional **QA Automation Engineer** designs a scalable Selenium test framework with reusable components, clean test structure, and automated reporting.

**Target Application:** SauceDemo
**Automation Tool:** Selenium WebDriver
**Programming Language:** Python
**Test Framework:** PyTest

---

# Key Features

* Page Object Model (POM) architecture
* Modular and maintainable code structure
* Automated HTML test reports
* Reusable driver setup
* Configuration-based environment setup
* Easy integration with CI/CD tools
* Scalable framework for additional tests

---

# Project Architecture

```
saucedemo-automation
│
├── tests
│   ├── test_login.py
│   ├── test_add_to_cart.py
│   └── test_checkout.py
│
├── pages
│   ├── login_page.py
│   ├── inventory_page.py
│   └── checkout_page.py
│
├── utils
│   ├── driver_factory.py
│   └── config.py
│
├── reports
│
├── screenshots
│
├── conftest.py
├── requirements.txt
└── pytest.ini
```

---

# Technology Stack

| Tool               | Purpose                             |
| ------------------ | ----------------------------------- |
| Python             | Programming language                |
| Selenium WebDriver | Browser automation                  |
| PyTest             | Test execution framework            |
| PyTest HTML        | HTML report generation              |
| WebDriver Manager  | Automatic browser driver management |

---

# Prerequisites

Before running the automation tests, ensure the following are installed:

* Python (3.8 or higher)
* Google Chrome browser
* Git (optional)

Verify installation:

```
python --version
pip --version
```

---

# Installation

Clone the repository:

```
git clone https://github.com/yourusername/saucedemo-automation.git
```

Navigate to the project directory:

```
cd saucedemo-automation
```

Install dependencies:

```
pip install -r requirements.txt
```

---

# Configuration

The test environment configuration is defined in:

```
utils/config.py
```

Example configuration:

```
BASE_URL = "https://www.saucedemo.com/"
USERNAME = "standard_user"
PASSWORD = "secret_sauce"
BROWSER = "chrome"
```

You can modify credentials or base URL here if needed.

---

# Test Scenarios Covered

### 1. Login Test

Verify that a registered user can successfully log in using valid credentials.

### 2. Add Product to Cart

Verify that a user can add a product to the shopping cart.

### 3. Checkout Process

Verify that the user can complete the checkout information step.

---

# Running Tests

Execute all tests using PyTest:

```
pytest
```

Run a specific test:

```
pytest tests/test_login.py
```

Run tests with detailed output:

```
pytest -v
```

---

# Test Reports

After execution, a detailed HTML report is automatically generated.

Report location:

```
reports/report.html
```

The report contains:

* Test execution summary
* Pass/Fail status
* Execution duration
* Error details (if any)

Open the report in any browser to view results.

---

# Page Object Model (POM)

The framework uses the **Page Object Model design pattern** which separates page logic from test logic.

Benefits include:

* Better code maintainability
* Reusability of page methods
* Reduced code duplication
* Cleaner test scripts

Each page of the application has its own class inside the **pages/** directory.

---

# Screenshots on Failure (Future Enhancement)

The framework structure supports adding automatic screenshots when tests fail. Screenshots can be stored in the **screenshots/** directory for debugging purposes.

---

# Continuous Integration (Optional)

This framework can easily integrate with CI/CD tools such as:

* Jenkins
* GitHub Actions
* GitLab CI

Example Jenkins pipeline stages:

1. Pull latest code
2. Install dependencies
3. Execute PyTest
4. Publish HTML report

---

# Best Practices Implemented

* Page Object Model architecture
* Configurable test environment
* Separation of test logic and page logic
* Automated reporting
* Modular and scalable project design

---

# Future Improvements

Possible enhancements to the framework include:

* Allure advanced reporting
* Parallel test execution
* Docker-based execution
* Cross-browser testing
* Logging integration
* Screenshot capture on test failure

---

# Author

QA Automation Framework Example
Designed following industry-level QA automation practices.

---

## License

This project is licensed under the MIT License – see the LICENSE file for details.