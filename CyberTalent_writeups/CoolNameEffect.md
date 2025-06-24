# Challenge - Cool Name Effect

- **Difficulty**: Easy  
- **Vulnerability**: PACKER JavaScript Obfuscation

## 🔍 Initial Analysis
- Suspicious `<script>` using PACKER by Dean Edwards.

## ⚔️ Exploitation
1. Copy and modify obfuscated JS to output decoded source (`console.log(p)`).
2. Use Node.js to evaluate the decoded source.
3. Identify and extract the flag or credential from the revealed logic.