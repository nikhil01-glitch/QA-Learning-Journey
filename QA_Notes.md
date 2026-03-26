
# QA Learning Notes

These are my personal notes while learning software testing concepts.

---

## What is Software
Software is basically a set of instructions or programs that tell a computer what to do.  
Examples include mobile apps, websites, operating systems, etc.

---

## What is QA (Quality Assurance)
QA focuses on making sure the software is built with good quality.  
It involves processes, testing methods, and practices that help prevent defects.

In simple terms → QA ensures the final product works correctly and meets requirements.

---

## SDLC (Software Development Life Cycle)

SDLC describes the stages used to build software.

Typical phases:

1. Requirement gathering  
2. Design  
3. Development  
4. Testing  
5. Deployment  
6. Maintenance

Testing mainly happens after development but QA involvement can start earlier.

---

## SDLC Models

### Waterfall Model
A linear approach where each phase happens one after another.

Requirement → Design → Development → Testing → Deployment

Simple but not very flexible if requirements change.

---

### Spiral Model
A risk-driven model where development happens in repeated cycles (spirals).  
Each cycle includes planning, risk analysis, development, and testing.

---

### V Model (Verification & Validation Model)

Testing activities are planned alongside development phases.

Example:

Requirement → Acceptance testing  
System design → System testing  
Module design → Integration testing  
Coding → Unit testing

This model emphasizes testing at every stage.

---

## Static vs Dynamic Testing

Static Testing
→ Checking documents, design, or code **without executing the program**.

Dynamic Testing
→ Actually running the software and checking its behavior.

---

## Static Testing Techniques

### Review
A general evaluation of documents or code by team members.

### Walkthrough
The author explains the document or code step by step to others.

### Inspection
A more formal review process where defects are identified systematically.

---

## Testing Approaches

### Black Box Testing
Testing software functionality **without knowing the internal code**.

Focus is on inputs and expected outputs.

---

### White Box Testing
Testing internal logic and code structure.

Usually done by developers or testers who understand programming.

---

### Grey Box Testing
Combination of black box and white box testing.
Tester has partial knowledge of internal structure.

### What is Software Testing?
Software testing is basically the process of checking whether a software application works the way it's supposed to. We do this to find bugs before the product reaches the end user. Testing also helps build confidence that the software meets the requirements it was built for.

---

### 1. Unit Testing
Unit testing is the most basic level of testing. Here we test individual components or functions of the code — one piece at a time, in isolation.

**Example:** If a developer writes a function to calculate the total price of items in a cart, unit testing would check whether that specific function gives the correct output for different inputs.

**Key points:**
- Done mostly by developers, not testers
- Happens during the development phase
- Tools commonly used: JUnit (Java), PyTest (Python), NUnit (.NET)
- Catches bugs early which makes fixing them cheaper

---

### 2. Integration Testing
Once individual units are tested, they need to work together. Integration testing checks whether different modules or components of the system work correctly when combined.

**Example:** Checking if the login module correctly communicates with the database module.

**Two common approaches:**
- **Big Bang** — integrate all modules at once and test together
- **Incremental** — integrate and test one module at a time (more practical)

**Key points:**
- Focuses on interaction between modules, not individual units
- Finds issues like data mismatch, API failures, wrong data flow
- Done after unit testing

---

### 3. System Testing
System testing is where we test the complete, fully integrated application as a whole. This is the stage where the software is tested against the actual requirements. Done by the QA team, not developers.

**Analogy:** Unit testing checks the engine, integration testing checks if the engine connects to the wheels, and system testing checks if the entire car actually drives properly.

---

### a) Functional Testing
Functional testing checks whether each feature of the application works as per the requirement. We basically give an input and verify the output.

**Example:** Testing the "Forgot Password" feature — enter email, check if OTP is received, check if password resets successfully.

**Key points:**
- Based on business requirements
- Black box testing — tester doesn't need to know the internal code
- Most common type of testing in day-to-day QA work

---

### b) GUI Testing (Graphical User Interface Testing)
GUI testing checks everything the user sees and interacts with on the screen. This includes buttons, text fields, menus, images, alignment, colors, fonts, and overall look and feel.

**Example:** Checking if the Submit button is correctly placed, font size is consistent across pages, and all images load properly.

**What we check:**
- All UI elements are present and visible
- Buttons and links are working
- Layout doesn't break on different screen sizes
- Color contrast and font readability
- Error messages are displayed correctly

---

### c) Usability Testing
Usability testing checks how user-friendly the application is. The goal is to see whether a real user can easily understand and use the software without confusion. This is less about whether the feature works and more about whether it's easy to use.

**Example:** Can a first-time user figure out how to place an order on an e-commerce site without any help? Are the navigation menus intuitive?

**Key points:**
- Sometimes done with real users, not just testers
- Focuses on user experience (UX)
- Looks at how many clicks to complete a task, are error messages clear, is the flow logical

---

### d) Non-Functional Testing
Non-functional testing checks how the system performs rather than what it does. It covers aspects like speed, reliability, scalability, and security.

**Main types:**
- **Performance Testing** — checks response time and stability under expected load
- **Load Testing** — checks behavior when many users are using the system simultaneously
- **Stress Testing** — pushes the system beyond its limits to see when and how it breaks
- **Scalability Testing** — checks if the system can handle growth in users or data
- **Compatibility Testing** — checks if the app works on different browsers, devices, and OS

---

### e) Security Testing
Security testing checks if the application is protected against threats, unauthorized access, and data breaches.

**Example:** Checking whether a normal user can access the admin panel, whether sensitive data like passwords are encrypted, whether the system is vulnerable to SQL injection.

**What security testing looks for:**
- Authentication and authorization flaws — can someone log in without correct credentials?
- SQL Injection — can a hacker manipulate the database through input fields?
- XSS (Cross-Site Scripting) — can malicious scripts be injected into the app?
- Data encryption — is sensitive data stored and transmitted securely?
- Session management — does the session expire after logout?

Security testing is especially critical for banking, healthcare, and e-commerce applications.

---

*Notes by Nikhil | QA Learning Journey | 2026*