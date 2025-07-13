# Comprehensive Site-Wide Audit Prompt

## Background

A thorough site-wide audit identifies critical issues that impact security, maintainability, performance, and user experience. This audit should examine both technical implementation and user-facing elements to ensure the site meets modern standards and best practices.

## Audit Instructions

Perform a comprehensive analysis of the provided website/application, examining the following areas:

### Security Assessment

- **Vulnerability Analysis**: Identify common security flaws (XSS, CSRF, SQL injection, insecure authentication)
- **Data Protection**: Review encryption, secure data transmission, and sensitive information handling
- **Access Controls**: Evaluate user permissions, authentication mechanisms, and authorization flows
- **Dependencies**: Check for outdated libraries with known vulnerabilities
- **Headers & Configuration**: Assess security headers, HTTPS implementation, and server configuration

### Code Quality & Standards

- **Consistency**: Flag inconsistent coding styles, naming conventions, and formatting across files
- **Architecture**: Identify structural issues, code duplication, and poor separation of concerns
- **Performance**: Spot inefficient algorithms, memory leaks, and resource-heavy operations
- **Documentation**: Evaluate code comments, README files, and technical documentation quality
- **Error Handling**: Review exception management and logging practices

### UI/UX Evaluation

- **Accessibility**: Test compliance with WCAG guidelines and screen reader compatibility
- **Responsive Design**: Check mobile compatibility and cross-device functionality
- **Navigation**: Assess information architecture and user flow clarity
- **Visual Consistency**: Identify design inconsistencies and branding violations
- **Load Times**: Evaluate page speed and user experience impact

### Technical Infrastructure

- **Performance Metrics**: Analyze loading speeds, caching strategies, and optimization opportunities
- **SEO Implementation**: Review meta tags, structured data, and search engine optimization
- **Browser Compatibility**: Test functionality across different browsers and versions
- **Database Optimization**: Examine query efficiency and data structure design

## Output Format

For each identified issue, provide:

1. **Severity Level** (Critical/High/Medium/Low)
2. **Specific Location** (file paths, line numbers, URLs)
3. **Description** of the problem
4. **Potential Impact** on users/security/performance
5. **Recommended Solution** with implementation steps
6. **Priority Ranking** for remediation order

Organize findings by category and include an executive summary with the most critical issues requiring immediate attention.
