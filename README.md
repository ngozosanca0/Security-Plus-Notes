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

## Day 4

NON-REPUDIATION 
- means a person cannot deny performing an action.
- real world example: think about hospital systems. If someone updates a patient record:
•The username is recorded.
•The time is recorded.
•The action is recorded.
- The user can't later deny making the change.
- That's non-repudiation.
- it matters because companies need accountability, audit trail and evidence.
- without non-repudiation, fraud investigations become difficult, insider threats become harder to trace. 


LEAST PRIVILEGE 
- means giving a user only the minimum level of access they need to do their job, nothing more.
- core idea: if you don't need it, you don't get it. 
- real world example: doctor can view patient records, receptionist cannot book appointments only, cleaner has no access to patient data. 
- even though all work in the same building, they do not all have the same access.
- that is least privilege. 
- it exists to reduce risk . 
- if an account is compromised, attacker only gets limited access, thus damage is reduced. 

ZERO TRUST
- means never trust automatically, always verify everything.
- even if a user or device is inside the network, it is not trusted by default.
- Traditional thinking says “If you are inside the company network, you are trusted.”
- but zero trust thinking says: “It doesn’t matter where you are, inside or outside, you must prove you are safe every time.”
- Zero Trust exists because modern networks are: cloud-based, remote work enabled, mobile device heavy, constantly under attack
- Hackers often: steal internal credentials, move inside networks and hide inside “trusted” environments.
- so companies assume: “Breach is already possible.”
- core idea: trust no one, verify everything. 

DEFENSE IN DEPTH
- means using multiple layers of security instead of relying on just one protection.
- core idea: If one security control fails, another one is still there.
- example: think of a bank vault, to steal money, a robber must pass the fence, security guard, locked doors, alarm system, CCTV, vault lock
- Each layer slows or stops the attacker.
- its important because no security control is perfect
- firewalls can be bypassed, Passwords can be stolen, users can click phishing links, and antivirus can miss malware.
- core idea: if one security control fails, others still protect the system. 

ACTIVE DIRECTORY 

ORGANIZATIONAL UNIT
- is like a folder that helps you organize users, computers, and groups inside a company.
- think of Active Directory as a filing cabinet:
• Domain = The entire company
• OU = A department's folder
• Users, Computers, Groups = The files inside that folder
- we use OUs for organisation
- organisation is keeping everything nest and easy to find.
- instead of havjng 1000 users in one place, you can separate them by department, location, job role.
- Again we use OUs to apply group policies. 
- meaning we can apply rules to everyone inside an OU.
- lastly we use OUs to delegate administration
- meaning you can give someone control over only their department. 
- example: HR manager can reset HR passwords but they cannot touch IT accounts.
- all in all: OU is a container within Active Directory used to organize users, computers, and groups. It helps administrators manage resources, apply Group Policies, and delegate administrative permissions efficiently.


