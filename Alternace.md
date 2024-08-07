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

