# HTTP Security Incident Analysis (Tcpdump Log Project)

## Overview
This project analyzes a simulated cybersecurity incident involving unauthorized access to a web server and malicious code injection. The investigation was conducted using network traffic analysis concepts.

## Objective
Identify the attack method, understand how the system was compromised, and recommend a mitigation strategy.

## Network Protocol Involved
- HTTP (Hypertext Transfer Protocol)

The attacker exploited HTTP by redirecting users to a malicious website and delivering harmful files.

## Incident Summary
A former employee performed a brute force attack on the administrative account by repeatedly attempting common/default passwords.

Once access was gained:
- The attacker logged into the admin panel
- Modified the website’s source code
- Injected a malicious JavaScript function
- Prompted users to download a file disguised as legitimate content

After downloading:
- Users were redirected to a fake website
- Systems slowed down, indicating malware infection

## Evidence of Compromise
- Multiple failed login attempts (brute force behavior)
- Unauthorized admin access
- Website code modification
- User complaints about forced downloads and redirects

## Attack Type
- Brute Force Attack
- Malware Injection
- Social Engineering (tricking users to download files)

## Impact
- Compromised user systems
- Loss of trust in the website
- Potential data exposure

## Remediation Recommendation
Implement account lockout policies:

- Limit login attempts (e.g., 5 tries max)
- Temporarily lock accounts after failed attempts
- Enforce strong password policies

## Additional Security Improvements
- Enable Multi-Factor Authentication (MFA)
- Monitor logs for unusual login activity
- Use HTTPS instead of HTTP
- Conduct regular security audits

## Conclusion
This incident demonstrates how weak authentication controls can lead to full system compromise. Strengthening login security and monitoring access logs are critical to preventing similar attacks.