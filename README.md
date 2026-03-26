# Factory Maintenance Secure App

A production-ready factory maintenance tracking system. It includes fixes for syntax errors, robust security enhancements such as session hardening, safe file uploads with .htaccess protection, strict input validation (allow-listing), secure logging practices, and absolute path routing to ensure scalability and enterprise-level reliability.

## Features
- Prevented SQL Injection via strict PDO Prepared Statements
- Mitigated XSS via centralized `htmlspecialchars` encoding
- Protected against CSRF using cryptographically secure tokens
- Hardened session management (HttpOnly, SameSite, UseOnlyCookies, Session ID regeneration)
- Secure log management via isolated directories and `.htaccess` access blocking
- Robust file upload handling with strict extension and MIME-type validation, stored in non-executable directories
- Mass Assignment prevention by using allow-lists for status updates
- Multi-language support (TH, EN, JP, CN)
- Responsive, clean UI for dashboards and admin panels