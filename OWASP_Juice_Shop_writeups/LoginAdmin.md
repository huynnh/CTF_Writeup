# Juice Shop Writeup: Login Admin

## Challenge Overview
**Title**: Login Admin  
**Category**: Injection  
**Difficulty**: ⭐⭐⭐⭐ (4/6)  
**Goal**: Log in with the administrator's user account.

## Exploit

### Step 1: Access login page
![The screenshot of the login page.](/assets/images/LoginAdmin_1.png)  

### Step 2: Insert SQL query into Email and Password fields
* Use the basic SQL Injection query.  
`' OR 1=1 --`  

![The screenshot of the login page is exploited.](/assets/images/LoginAdmin_2.png)  

## Explanation
This challenge was resolved by utilizing an SQL Injection to bypass the website's authentication. By inject `' OR 1=1 --` make SQL return `TRUE` result allow attacker login without valid credentials.