# INTERFACES
- IUser
    - TryLogin(identifier, password)

# CLASSES
- User : IUser
    - string SSN
    - string Password
    - string Name
    - Clearance Clearance.Minimal
    - TryLogin()

- Admin : IUser
    - string Email
    - string Password
    - string Name
    - Clearance Clearance.High
    - TryLogin()

- Patient
    - string SSN
    - string Name
    - enum Region
    - Clearance Clearance;
    public Patient()
    {
        Clearance clearance = Clearance.Low;
    }

- Personnel
    - string SSN
    - string Name
    - enum Region
    - enum JobTitle
    - Clearance Clearance.Medium

- Journal
    - string ID
    - Patient Patient
    - Personnel Personnel
    - Dictionary<DateTime, string> // Date, BodyText
    - Read Permission ?

- HealthCareSystem
    - List<IUser>
    - List<Journal>
    - List<Region>
    - List<Patient>
    - List<Personnel>

- Region

# ENUM
- Region
    - Halland         
    - Norrbotten
    - Västra Götaland
    - Skåne

- JobTitle
    - Nurse
    - Anesthesiologist
    - Surgeon
    - Janitor
    - Sub-nurse

- Clearance
    - Minimal
        - 
    - Low
        - 
    - Medium
        - 
    - High
        - 
    - Maximal
        - 
if (clearance == Clearance.Minimal)

- Menu

# Persistent Storage
- .csv (id~text~date) seperator: "~"

- iuser.csv
    - ID~Password~Clearance~Name

- patients.csv
    - ID~Clearance~Name

- personnel.csv
    - ID~Clearance~Name
 
- journals.csv
    - JID~PaID~PeID~Dictionary

- entries.csv
    - JID~Date~Text

j04, 2025, blabla
j02, 2025, blabla
j03, 2025, blabla
j01, 2025, blabla
j02, 2025, blabla
j03, 2025, blabla


# Discussion

Admin: 
- Functionality
    - 

if (IUser user is Patient pa || )
else if (IUser user is Personnel pe)

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