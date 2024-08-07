# Job Search for Apprenticeship and Internship

### Classes and Methods

#### 1. Class: User

- **Properties:**
  - `id`
  - `name`
  - `email`
  - `password`
********
- **Methods:**
  - `register()`
  - `login()`
  - `logout()`

#### 2. Class: Student (inherits from User)

- **Properties:**
  - `resume`
  - `coverLetter`
  - `skills` (List of skills)
  - `experiences` (List of experiences)

- **Methods:**
  - `applyForJob()`
  - `searchForJob()`

#### 3. Class: Company (inherits from User)

- **Properties:**
  - `NIF_STAT` (Tax Identification Number)

- **Methods:**
  - `postJob()`
  - `searchForJob()`

#### 4. Class: Post

- **Properties:**
  - `id`
  - `title`
  - `description`
  - `publicationDate`

- **Methods:**
  - `displayDetails()`
  - `editJob()`
  - `deleteJob()`

#### 5. Class: Skill

- **Properties:**
  - `id`
  - `name`
  - `level` (ENUM: beginner, intermediate, expert)

#### 6. Class: ProfessionalExperience

- **Properties:**
  - `id`
  - `jobTitle`
  - `company` (Previous)
  - `startDate`
  - `endDate`
  - `description`

#### 7. Class: Application

- **Properties:**
  - `id`
  - `applicant` (Component)
  - `jobOffer`
  - `applicationDate`
  - `status` (ENUM: in progress, accepted, rejected)

- **Methods:**
  - `updateStatus()`

### 8. **JobOffer:**

- `id`
- ``title``
- ``description``
- ``location``
- ``publicationDate``
- ``expirationDate``
- ``requiredSkills``
- ``User`` (Component)

Certainly! Below is a class definition for `CV` (Curriculum Vitae) that includes typical properties and methods relevant to a CV in the context of job applications.

### Class: CV

- **Properties:**
  - `id` (Unique identifier for the CV)
  - `student` (Reference to the Student who owns the CV)
  - `personalInformation` (e.g., name, contact information)
  - `education` (List of educational qualifications)
  - `skills` (List of skills)
  - `workExperience` (List of ProfessionalExperience)
  - `projects` (List of projects)
  - `certifications` (List of certifications)

- **Methods:**
  - `addEducation(degree, institution, startDate, endDate, description)`
  - `addSkill(skill)`
  - `addWorkExperience(jobTitle, company, startDate, endDate, description)`
  - `addProject(projectTitle, description)`
  - `addCertification(certificationName, issuingOrganization, dateIssued)`
  - `updatePersonalInformation(name, contactInfo)`
  - `display()` (Displays the CV in a user-friendly format)
