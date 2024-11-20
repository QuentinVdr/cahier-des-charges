# Cours de cahier des charges

## exo 1

Diagramme de flux d'utilisateur pour envoyer un mail avec piece jointe

```mermaid
graph TD
    A@{ shape: sm-circ, label: "Small start" } --> B[Écrire un mail]
    B --> C{Ajouter une piece jointe}
    C --> |oui| D[Télécharger piece jointe]
    C --> |non| E[Envoyer le mail]
    D --> E
    E --> F@{ shape: framed-circle, label: "Stop" }
```

## exo 2

A partir du premier TP pour pour le Gestionnaire Électronique de Documents.
Créer le diagramme de flux d'utilisateur pour ajouter un document.

```mermaid
graph TD
    A(Début) --> B[Collecte des besoins métiers]
    B --> C{Les besoins sont-ils clairs et complets ?}
    C -- Oui --> E[Analyse des exigences]
    C -- Non --> D[Clarification et complément des besoins]
    D --> B
    E --> F[Définition des objectifs et du périmètre du projet]
    F --> G[Évaluation des processus existants]
    G --> H{Les processus actuels sont-ils efficaces ?}
    H -- Oui --> I[Identification des améliorations potentielles]
    H -- Non --> J[Redéfinition des processus]
    I --> K[Développement des spécifications fonctionnelles]
    J --> K
    K --> L[Choix de la solution GED]
    L --> M{Solution existante ou développement sur mesure ?}
    M -- Existante --> N[Sélection d'une solution sur le marché]
    M -- Sur mesure --> O[Développement d'une solution personnalisée]
    N --> Q[Implémentation de la GED]
    O --> Q
    Q --> R[Tests et validation]
    R --> S{Les tests sont-ils concluants ?}
    S -- Oui --> T[Formation des utilisateurs]
    S -- Non --> U[Corrections et ajustements]
    U --> Q
    T --> V[Mise en production]
    V --> W[Suivi et support post-implémentation]
    W --> X(Fin)
```
