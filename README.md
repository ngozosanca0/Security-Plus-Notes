# Security-Plus-Notes


## Day 1: Security Controls 

TYPES 
- Preventive controls stop attacks before they happen.
- Detective controls identify events and incidents when they happen. 
- Corrective controls help restore systems after an attack.
- Deterrent Controls discourage attacks to make attackers think twice before attacking. 
- Compensating controls are substitute security controls used when the main control cannot be used.
- Directive Controls tell people what they should do to guide behavior and enforce expectations. 

CATEGORIES 
- Technical controls are tools and technology doing the work
- Physical controls are controls that physically stop or limit access to systems or facilities. 
- Operational controls security controls carried out by humans.
- Managerial controls are high level policies, governance and risk decisions. 

## Day 2: CIA TRIAD 

CONFIDENTIALITY 
- Only authorized people should access the data, preventing unauthorized access. 
- the goal is to keep information private. 
- Examples: Passwords, MFA, Patient records.
- real life example: Your banking passwords should only be known by you.
- if confidentiality is broken, data leaks and there will be unauthorized access. 

INTEGRITY
- Data must remain accurate, trustworthy, and unchanged unless authorized.
- the goal is to protect data from unauthorized modification 
- real world examples: a bank should not change from R5000 to R50000.
- if integrity is broken, there is data tampering, corruption. 

AVAILABILITY 
- systems and data must be accessible when needed. 
- the goal is to ensure systems stay operational. 
- real world example: Hospital system must stay online 24/7.

CIA TRIAD SIMPLE EXAMPLE USING BANK VAULT
- Confidentiality: Only authorized people open the vault
- Integrity: Money inside is untouched and accurate
- Availability: Vault can be accessed when needed

## Day 3: AAA and Active Directory 

AAA

AUTHENTICATION 
- Verifying your identity.
- the system checks "are you really who you claim to be"
- real world example: you swipe your employee badge and enter password
- the system verifies your badge and password,  that is authentication. 

AUTHORIZATION 
- determining what you are allowed to access or do.
- real life example: HR Manager can access salaries and employee records but receptionist cannot access those files.
- Both are authenticated, but their authorization differs.

ACCOUNTING 
- Tracking and recording user activity. 
- real-world example: an administrator deletes files at 2AM, accounting logs show who did it, when and from which device.
- accounting matters because it helps with investigations, compliance, detecting insider threats and non-repudiation. 


ACTIVE DIRECTORY 

WINDOW DOMAIN 
- is a way to connect all company computers to one central management system. 
- instead of each computer being independent, they all “report” to one main server.
- that main server is called the: Domain Controller (DC).

DOMAIN CONTROLLER
- the server that runs active directory
- it stores: User accounts, Passwords, Permissions, Security policies, Device rules, Access rights. 
- it controls all computers connected to the domain.

ACTIVE DIRECTORY
- is the database/service running on the Domain Controller.
- it stores all network information.
- it keeps track of: Users. 
- Examples: John, Sarah, Admin1, FinanceManager
- It stores their: Usernames, Passwords, Access permissions, Roles.
• It knows every company computer: Reception-PC. Finance-PC, CEO-Laptop, HR-PC. 
• You can organize users into departments: HR, IT, Finance, Sales. Then apply rules to the whole group.

