# Challenge - Admin has the power

**Difficulty**: Easy  
**Vulnerability**: Broken Access Control

## 🔍 Initial Analysis
Login as `support` works.
Cookie includes a `role` parameter.

## ⚔️ Exploitation
Use Buite Suite to catch the request

![request image](/resources/img-1.1.png)

Change `role=support` to `role=admin` while keeping the same PHPSESSID.
Result: Gain unauthorized admin access.

## ⚠️ Impact
Serious Broken Access Control vulnerability (Top 1 OWASP).
Allows privilege escalation without proper server-side authorization.

## 🛠️ Remediation
Never store roles in cookies.
Always validate roles server-side.