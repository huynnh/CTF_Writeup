# Challenge - Cool Name Effect

**Difficulty**: Easy  
**Vulnerability**: PACKER JavaScript Obfuscation

## 🔍 Initial Analysis
Suspicious code in `<script>` tag is PACKER JavaScript Obfuscation.  
![PACKER JavaScript Obfuscation](../assets/images/CyberTalent/img-4.1.png)

Also in `<script>` tag have a function to decrypt it.  
![Decrypt Function](../assets/images/CyberTalent/img-4.2.png)

## ⚔️ Exploitation
Install NodeJS

Copy the decrypt function into a `.js` file.  
![Decrypt Function](../assets/images/CyberTalent/img-4.3.png)

Change the `return p;` to `console.log(p)` and execute it with NodeJS.  
After execute successfully, copy all output into the second `.js` file. This output is the origin code.

We observe the JS code, there is a suspicious function:
![suspicious function](../assets/images/CyberTalent/img-4.4.png)

Adjust code a little bit like this:  
![suspicious function](../assets/images/CyberTalent/img-4.5.png)  

Then execute the second `.js` file with NodeJS.