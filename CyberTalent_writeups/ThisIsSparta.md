# Challenge - This is Sparta

- **Difficulty**: Easy  
- **Vulnerability**: Exposed Client-Side Logic

## 🔍 Initial Analysis
- Server: Nginx 1.27.1, PHP 7.2.34
- JavaScript code in the response contains obfuscated login check.

## ⚔️ Exploitation
- Use **CyberChef** to decode the JavaScript array and variables.
- Logic shows credentials are hardcoded: `username = Cyber`, `password = Talent`.

## ⚠️ Impact
- Complete bypass of login mechanism.
- Exposes sensitive credentials in client-side JS.

## 🛠️ Remediation
- Authentication must be handled on the server.
- Never expose credentials or logic in client-side code.
