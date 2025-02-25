
## **Documentation of Static Code Anaylysis in Java CI Checks**

| **Author** | **Created on** | **Version** | **Last updated by**|**Last Edited On**|**Level** |**Reviewer** |
|------------|---------------------------|-------------|----------------|-----|-------------|-------------|
| Nikita Joshi|  26-02-2025           | v1         | Nikita Joshi    |26-02-2025    |  internal review | komal jaiswal | 

## **Introduction**

Continuous Integration (CI) is a key practice in software development where code changes are frequently merged, built, and tested. Static code analysis is a method to examine code without executing it, helping to find errors, bugs, and security issues. Combining CI with static code analysis ensures better code quality and fewer vulnerabilities in Java projects.

___

## What is Static Code Analysis?
Static code analysis is the process of reviewing code without running it. It helps detect errors, bugs, and security vulnerabilities by analyzing the code structure and patterns.

---

## Why Use Static Code Analysis in CI?

| **Reason**              | **Description**                                                                 |
|--------------------------|---------------------------------------------------------------------------------|
| **Early Bug Detection**  | Catch issues during development before runtime testing.                         |
| **Enhanced Security**    | Identify vulnerabilities early to reduce risks.                                |
| **Improved Code Quality**| Enforce coding standards and best practices.                                   |
| **Reduced Maintenance Costs** |	Clean code with fewer bugs reduces long-term maintenance expenses.|
|**Improved Team Collaboration** |	Consistent code style and fewer errors make teamwork easier and more effective.|
---

## Tools for Static Code Analysis

| **Tool**               | **Description**                                                                 |
|-------------------------|---------------------------------------------------------------------------------|
| **SonarQube**           | Supports multiple languages and offers extensive integration options.           |
| **Checkstyle**          | Focuses on enforcing Java coding standards.                                    |
| **PMD**                 | Detects unused variables, bugs, and other issues.                              |
| **FindBugs/SpotBugs**   | A tool for finding bugs in Java programs.                                      |

---



## Comparison of Tools

| **Feature**            | **SonarQube** | **Checkstyle** | **PMD** | **FindBugs/SpotBugs** |
|-------------------------|---------------|----------------|---------|-----------------------|
| **Language Support**    | Multi         | Java           | Multi   | Java                  |
| **Security Checks**     | Yes           | No             | Yes     | Limited               |
| **Integration Options** | Extensive     | Moderate       | Good    | Limited               |
| **Ease of Use**         | Moderate      | High           | High    | High                  |
| **Community**           | Large         | Medium         | Medium  | Large                 |
| **Cost**                | Paid/Free     | Free           | Free    | Free                  |
| **User Interface**      | Advanced      | Basic          | Basic   | Basic                 |


## **Conclusion**

Static code analysis tools in Java help identify issues early, improving code quality, security, and maintainability, which reduces long-term costs. However, they should be paired with dynamic analysis and other testing methods for comprehensive code quality.


## **Contact Information**

| **Name** | **Email address**            | **Github ID**
|----------|-------------------------------|-------------------|
| Nikita joshi    | Nikita.Joshi@mygurukulam.co    | https://github.com/jnikita19  |


## References
- [Static Code Analysis](https://www.techtarget.com/whatis/definition/static-analysis-static-code-analysis)
- [SonarQube for Static Code Analysis](https://www.sonarsource.com/learn/static-code-analysis-using-sonarqube/)
- [List of Static Code Analysis Tools](https://en.wikipedia.org/wiki/List_of_tools_for_static_code_analysis)
- [POC for Static Code Analysis]()
