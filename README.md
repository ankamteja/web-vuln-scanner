# Web Vulnerability Scanner

An automated web application vulnerability scanner that crawls target URLs and tests for common security vulnerabilities via payload injection.

## Features

- Endpoint crawler with multi-threaded requests
- Vulnerability detection: SQL Injection, XSS, Open Redirects, Path Traversal
- Payload-based active testing (not pattern matching)
- Structured JSON report output
- CLI interface with configurable options

## Supported Vulnerability Checks

| Vulnerability | Method |
|---|---|
| SQL Injection | Error-based & boolean payload injection |
| Cross-Site Scripting (XSS) | Reflected payload detection |
| Open Redirect | Parameter manipulation |
| Path Traversal | Directory escape sequences |

## Usage

```bash
python scanner.py -u http://target.com -o report.json
```

## Tested Against

- DVWA (Damn Vulnerable Web Application)
- HackTheBox machines

## Disclaimer

For authorized testing only. Do not use against systems you do not have permission to test.
