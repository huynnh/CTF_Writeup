# Challenge - This is Sparta

**Difficulty**: Easy  
**Vulnerability**: Exposed Client-Side Logic

## 🔍 Initial Analysis
Use Buite Suite to catch the request. There is a strange Javascript code in `<script>` tag:

![Strange JS code](/resources/img-2.1.png)

## ⚔️ Exploitation
Use **CyberChef** or any decrypt tools to decode the JavaScript array and variables.  
Logic shows credentials are hardcoded: `username = Cyber`, `password = Talent`.

## ⚠️ Impact
Complete bypass of login mechanism.  
Exposes sensitive credentials in client-side JS.

## 🛠️ Remediation
Authentication must be handled on the server.  
Never expose credentials or logic in client-side code.