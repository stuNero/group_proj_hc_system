# INTERFACES
- IUser
    - TryLogin(identifier, password)

# CLASSES
- User : IUser
    - string SSN
    - string Password
    - TryLogin()
- Admin : IUser
    - string Email
    - string Password
    - TryLogin()
- SysAdmin : Admin : IUser
    - TryLogin()
- Patient
- Personnel
- HCSystem

# ENUM

# Discussion
user1
- id
- email
- password
patient1
- namn
- id 
- Schedule
- 
personnel1
- namn
- id
- schedule

users.csv
- mv001, Max vemic
- aj001, Amir Jafari
- pc001, Pierino Corona

patients.csv
- mv001, journalListID
- aj001, journalistID
- pc001, journallistID

personnel.csv
mv001, Max 