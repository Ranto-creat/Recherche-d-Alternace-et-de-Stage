# Recherche d'alternace et stage

### Classes et Méthodes

#### 1. Classe : User

- **Propriétés :**
  - `id`
  - `nom`
  - `email`
  - `password`

- **Méthodes :**
  - `inscrire()`
  - `seConnecter()`
  - `seDeconnecter()`

#### 2. Classe : Etudiant (hérite de User)

- **Propriétés :**
  - `cv`
  - `lettreDeMotivation`
  - `competences` (Liste de compétences)
  - `experiences` (Liste d'expériences)

- **Méthodes :**
  - `postulerOffre()`
  - `rechercherOffre()`

#### 3. Classe : Entreprise (hérite de User)

- **Propriétés :**
  - `NIF_STAT`

- **Méthodes :**
  - `publierOffre()`
  - `rechercherOffre()`

#### 4. Classe : Post

- **Propriétés :**
  - `id`
  - `titre`
  - `description`
  - `dateDePublication`

- **Méthodes :**
  - `afficherDetails()`
  - `modifierOffre()`
  - `supprimerOffre()`

#### 5. Classe : Competence

- **Propriétés :**
  - `id`
  - `name`
  - `niveau` (ENUM : débutant, intermédiaire, expert)

#### 6. Classe : ExperienceProfessionnelle

- **Propriétés :**
  - `id`
  - `titrePost`
  - `entreprise` (Précédente)
  - `dateDebut`
  - `dateFin`
  - `description`

#### 7. Classe : Candidature

- **Propriétés :**
  - `id`
  - `candidat` (Composant)
  - `offreEmploi`
  - `dateCandidature`
  - `statut` (ENUM : en cours, accepté, rejeté)

- **Méthodes :**
  - `mettreAJourStatut()`

### 8. **OffreD_emploi :**

- ``id``
- ``titre``
- ``description``
- ``localisation``
- ``date_de_publications``
- ``date_d_expiration``
- ``competences_requise``
- ``User`` (Composant)

### Classe : CV

- **Propriétés :**
  - `id` (Identifiant unique pour le CV)
  - `student` (Référence à l'étudiant qui possède le CV)
  - `personalInformation` (par exemple, nom, informations de contact)
  - `education` (Liste des qualifications éducatives)
  - `skills` (Liste des compétences)
  - `workExperience` (Liste des expériences professionnelles)
  - `projects` (Liste des projets)
  - `certifications` (Liste des certifications)

- **Méthodes :**
  - `addEducation(diplôme, établissement, dateDébut, dateFin, description)`
  - `addSkill(compétence)`
  - `addWorkExperience(titrePoste, entreprise, dateDébut, dateFin, description)`
  - `addProject(titreProjet, description)`
  - `addCertification(nomCertification, organismeÉmetteur, dateDélivrance)`
  - `updatePersonalInformation(nom, informationsContact)`
  - `display()` (Affiche le CV dans un format convivial)
