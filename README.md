# Extended DNS Error (EDE) Support in Chrome

## Overview

Welcome to my repository! This project demonstrates my implementation of **Extended DNS Error (EDE)** support in Chrome's DNS stack. The main goal of this work is to enhance Chrome's DNS error handling capabilities by implementing RFC 8914 Extended DNS Errors, which provides more detailed information about why DNS queries are blocked or filtered.

For a detailed view of the changes, please see [Issue #1](https://github.com/Konikz/chrome-dns-ede/issues/1).

---

## Project Contribution to Chrome

### Key Changes

* **EDE Record Parsing:**  
Implemented a robust parser for Extended DNS Error records that handles both basic and structured error data formats. This allows Chrome to extract detailed error information from DNS responses.

* **Error Handling Integration:**  
Integrated EDE support into Chrome's DNS transaction handling, enabling the browser to process and respond appropriately to various types of DNS errors.

* **Configuration Options:**  
Added configuration options to control EDE processing behavior, allowing users and administrators to customize how Chrome handles different types of DNS errors.

### Implementation Details

The implementation includes:

* **New Files:**
  * `net/dns/dns_ede.h`: Header file defining the EDE record structure and parsing functions
  * `net/dns/dns_ede.cc`: Implementation of EDE parsing and error handling logic
  * `net/dns/dns_ede_unittest.cc`: Comprehensive unit tests for EDE functionality

* **Key Features:**
  * Parses EDE records from DNS responses
  * Handles structured DNS error data
  * Provides blocking detection for EDE error codes
  * Includes comprehensive unit tests
  * Integrates with Chrome's existing DNS infrastructure

---

## Testing & Feedback

The implementation includes comprehensive unit tests covering:
* Basic EDE record parsing
* Structured data handling
* Error code validation
* Invalid input handling

I welcome suggestions and contributions from the Chrome team and the broader community to refine this implementation. If you have insights on how to improve the code or enhance the functionality, I would love to collaborate and iterate on the implementation.

This process is an opportunity for me to **learn from experienced contributors, improve code quality, and better understand Chrome's architecture**. If you are reviewing this implementation and have any suggestions, feel free to comment on the GitHub discussion or reach out directly!

---

## About Me

**Hello, I'm Konikz – a recent Computer Science and Engineering graduate from India.**  
 Although I am new to open source, I am dedicated to refining my skills in distributed systems, cloud computing, and scalable software design. I am eager to contribute to high-impact projects and look forward to opportunities like Google Summer of Code (GSoC) to further develop my expertise.

---

## P.S.

As a newcomer to open source, I truly appreciate any feedback and guidance from the Chrome team and the community. This project represents my first major contribution to Chrome, and I am excited to learn and grow through collaboration.

\* **If you're reviewing this, your insights and suggestions would be invaluable in helping me refine this feature!**
