
Security Header Checker 

This repository contains a set of Python scripts designed to check the presence and configuration of security HTTP headers in web server responses.

Table of Contents
Installation
Scripts Overview
1. check_headers.py
2. check_specific_header.py
3. check_specific_headerr.py
4. enhanced_security_header_checker.py
5. security_headers_checker.py
6.spider.py

## Scripts

check_headers.py: Analyzes HTTP response headers for security settings.
check_specific_header.py: Checks for specific security headers in HTTP responses.
check_specific_headerr.py: Checks for specific security headers in HTTP responses using URLs from a file.
enhanced_security_header_checker.py: Performs enhanced security header checks on a given URL.
security_headers_checker.py: Checks for predefined security headers in the response headers of a specified URL.
spider.py: Web crawler to collect URLs for testing

## Supported Security Headers and Significance

The tool checks for the following security headers and explains their significance:

- **Content-Security-Policy (CSP)**: Specifies approved sources for content, protecting against XSS and data injection attacks.
- **X-XSS-Protection**: Enables or disables the browser's XSS protection.
- **Strict-Transport-Security (HSTS)**: Ensures that browsers only access a website over HTTPS, preventing protocol downgrade attacks.
- **X-Frame-Options**: Prevents clickjacking attacks by controlling if and how a page can be loaded within a frame or iframe.
- **X-Content-Type-Options**: Prevents browsers from MIME-sniffing a response away from the declared content type.
- **Referrer-Policy**: Controls how much referrer information is included with requests.

Each security header contributes to enhancing the security posture of a web application by mitigating specific types of attacks.

## Usage

To use the scripts, ensure you have Python installed. Install any required dependencies with:

### Prerequisites

- Python 3.x installed on your system.

### Installation

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/Cipherkrish69x/security-headers-tool.git
   cd security-headers-tool

Certainly! Let's create a README.md file tailored specifically to the scripts you've provided. We'll include descriptions, usage instructions, and details about each script.

---

# Security Headers Tool

This repository contains a collection of Python scripts designed to analyze and check security HTTP headers in web server responses.

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/Cipherkrish69x/security-headers-tool.git
   cd security-headers-tool
   ```

2. **Install Requirements:**

   Ensure you have Python 3 installed. Install the required Python packages using pip:

   ```bash
   pip install -r requirements.txt
   ```

## Scripts Overview

### 1. `check_headers.py`

This script checks the presence of specified HTTP headers in the response headers of a single URL.

**Usage:**

```bash
python3 check_headers.py --urls-file urls.txt --headers-file headers.txt --output-file results.json
```

- `--urls-file`: Path to a text file containing URLs to check.
- `--headers-file`: Path to a text file containing HTTP headers to verify.
- `--output-file`: (Optional) Path to save the JSON results.

### 2. `check_specific_header.py`

Checks the presence of a specific HTTP header in the response headers of multiple URLs.

**Usage:**

```bash
python3 check_specific_header.py
```

- You will be prompted to enter the header name and URLs separated by spaces.

### 3. `check_specific_headerr.py`

Similar to `check_specific_header.py`, but reads URLs from a file (`urls.txt`).

**Usage:**

```bash
python3 check_specific_headerr.py
```

- Reads URLs from the `urls.txt` file and prompts for the header name.

### 4. `enhanced_security_header_checker.py`

Performs enhanced security header checks on a single URL.

**Usage:**

```bash
python3 enhanced_security_header_checker.py <url> --output-file output.txt
```

- Replace `<url>` with the URL you want to check.
- Use `--output-file` to specify a file to save the results.

### 5. `security_headers_checker.py`

Checks for the presence and configuration of a set of predefined security headers in a given URL.

**Usage:**

```bash
python3 security_headers_checker.py
```

- You will be prompted to enter the URL you want to test.

## Author

- **Alla Krishna Vamsi Reddy** ([GitHub Profile](https://github.com/Cipherkrish69x))

---
