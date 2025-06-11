# Challenge - Iam Legend

- **Difficulty**: Easy  
- **Vulnerability**: JSFuck Obfuscation Leak

## 🔍 Initial Analysis
- Login page with obfuscated JavaScript (`JSFuck`).
- Server stack same as Challenge 2.

## ⚔️ Exploitation
- Use **de4js** tool to deobfuscate.
- Extracted condition: `user == Cyber && pass == Talent`.