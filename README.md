# Arts Tailor Shopee E-Commerce Website

## Overview
Arts Tailor Shopee is an e-commerce platform designed for showcasing and selling tailor-made fashion products. This specific repository contains the source code for a training extension of the website, which includes intentional vulnerabilities aimed at providing a practical exercise for penetration testers.

## Features
- **Product Listings**: Displays a variety of tailor-made fashion products.
- **Search Functionality**: Allows users to search for products.
- **Feedback Form**: Enables users to submit feedback about products and services.
- **User Authentication**: Manages user registration, login, and profile management.

## Intentional Vulnerabilities
For educational purposes, this version of the website includes two specific vulnerabilities designed to simulate common security issues in web applications:
1. **Sanitized Search Bar**: The search input is sanitized to demonstrate resistance to most XSS payloads.
2. **Vulnerable Feedback Form**: The `name` attribute in the feedback form is intentionally poorly sanitized, creating a potential for DOM-based XSS attacks.

## Installation and Setup
1. Clone the repository to your local machine.
2. Ensure you have [Apache2](https://httpd.apache.org/) installed to host the website.
3. Place the source code in the `/var/www/html` directory of your Apache server.
4. Configure the server with a static IP address (e.g., `10.72.24.5`) for consistency in testing.

## Usage
The website can be accessed locally via the configured static IP or through DNS mapping for more realistic testing (e.g., mapping `10.72.24.5` to `www.artsfashions.com` in your hosts file).

## Tools for Testing
- **Burp Suite Community Edition**: Recommended for executing penetration tests, particularly using the DOM Invader tool.
- **Virtual Machines**: The website should be hosted on an Ubuntu VM, with tests conducted from a Kali Linux VM.

## Contribution
Contributions to improve the website's functionality or enhance the educational aspect of the vulnerabilities are welcome. Please submit a pull request or open an issue to discuss proposed changes.

## Disclaimer
This website is designed for educational and training purposes only. It contains intentional security vulnerabilities and should not be deployed in a production environment or accessible from the public internet.

## License
[MIT License](LICENSE)

## Contact
For more information or queries, please contact the repository maintainers at [contact@artsfashions.com](mailto:contact@artsfashions.com).
