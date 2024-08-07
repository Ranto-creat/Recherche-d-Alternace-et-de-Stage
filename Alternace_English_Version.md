# Job Search for Apprenticeship and Internship

### Classes and Methods

#### 1. Class: User

- **Properties:**
  - `id`
  - `name`
  - `email`
  - `password`

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

