# Changelog — GAB. Guide Antécédents Bonus-Malus

## v1.3 — Succès & badges
*5 mars 2026*

### 🏅 Système de succès (34 badges)
Un système de badges est désormais intégré au GAB — accessible depuis la barre de navigation via le bouton *Succès*.

- **34 badges déblocables** répartis en 9 catégories : Moto, Contrat, Validation, Espaces de travail, Tableau, CRM, Contrôle vitesse, Fidélité et SGP
- **Toast animé** à l'écran à chaque nouveau badge débloqué
- **Vue d'ensemble** : grille de tous les badges — débloqués en couleur, verrouillés en grisé avec barre de progression
- **Badges liés à l'activité** : se débloquent automatiquement selon votre utilisation (dossiers enregistrés, validations effectuées, connexions quotidiennes, performance sur les retours SGP…)
- Les badges SGP (taux de validation 50 % / 70 % / 100 %, séries hebdomadaires) sont alimentés automatiquement par le Gestionnaire SGP

### Correctifs & améliorations
- Bouton **⋯ Options** dans la barre de navigation : regroupe Paramètres, Informations, Nouveautés, Imprimer et Thème en un seul menu déroulant
- Transmission des résultats SGP vers le GAB plus robuste (gestion multi-entrées, déclenchement à la reprise de focus)

---

## v1.2 — Gestionnaire SGP & alertes intégrées
*27 février 2026*

### 🆕 Gestionnaire de retours SGP (nouvel outil)
Un outil dédié au suivi des retours SGP est désormais disponible à l'adresse **GAB_SGP**, accessible directement depuis le menu (☰) du GAB.

- **Import rapide** : collez le tableau du mail SGP Outlook (Ctrl+A dans le corps du mail, Ctrl+C, puis Ctrl+V dans l'outil) — le tableau est analysé et structuré automatiquement
- **Suivi des corrections** : chaque ligne affiche le N° contrat, le statut de validation, l'action requise et la correction à apporter ; cochez les dossiers traités au fur et à mesure
- **Badges de statut** colorés par type d'action (Avenant, Validé, Résilié, Nullité…) et alerte visuelle rouge pour les dossiers non validés
- **Deadline automatique** : la date limite de traitement est détectée dans le mail et affichée avec une couleur d'alerte (rouge si dépassée, orange si proche)
- **Statistiques en temps réel** : compteurs *À traiter / Traités / Dossiers parfaits* mis à jour à chaque action
- **Archivage en un clic** : une fois tous les dossiers traités, le retour est copié dans le presse-papier (format tableau prêt pour Teams/mail) et archivé automatiquement
- **Historique** : les retours archivés restent consultables et récupérables depuis l'onglet *Historique SGP*
- **Onglets multi-imports** : plusieurs retours SGP simultanés gérés en parallèle avec onglets de navigation
- Purge automatique des imports de plus de **30 jours**

### 🔔 Alertes SGP dans le GAB
- **Point rouge** sur le bouton *Gestionnaire SGP* dans le menu (☰) dès qu'un retour est en attente — prioritaire sur le badge Nouveautés
- **Bannière quotidienne** discrète affichée une fois par jour sous le bandeau de mise à jour : indique le nombre de retours en attente et la deadline, cliquable pour ouvrir directement le gestionnaire ; fermable avec ✕

### Correctifs & améliorations
- Lien de navigation **GAB ↔ SGP** : retour vers le GAB depuis le Gestionnaire SGP, et accès au Gestionnaire depuis le menu du GAB
- Numéro de version affiché dans le menu du Gestionnaire SGP

---

## v1.1.8 — Espaces de travail
*26 février 2026*

### 🆕 Espaces de travail (3 slots simultanés)
- Travaillez sur **3 dossiers en parallèle** sans perdre vos données : 3 emplacements nommés librement côte à côte dans la barre de sauvegarde
- **Indicateur d'état** sur chaque espace (gris = vide, orange = non sauvegardé, vert = à jour)
- Protection contre le changement d'espace sans sauvegarde préalable
- Désactivable depuis les **Paramètres** si vous préférez le mode champ unique

---

## v1.1.7 — Impression & correctif alerte CRM
*26 février 2026*

### 🆕 Imprimer / PDF `[ALPHA]`
- Bouton **Imprimer / PDF** dans le menu (☰) pour générer une version imprimable du dossier
- ⚠️ La mise en page peut varier selon le navigateur — fonctionnalité en cours d'amélioration

### Correctif
- **Alerte perte de CRM** : l'alerte ne se déclenche désormais que si l'interruption de plus de 24 mois est présente **à la fin de la période saisie** — les interruptions anciennes suivies d'une reprise de couverture ne génèrent plus de fausse alerte

---

## v1.1.1 → 1.1.6 — Stabilisation
*25 février 2026*

- Corrections mineures sur la détection de mise à jour
- Harmonisation visuelle mode clair / sombre

---

## v1.1 — Validation guidée, Menu principal & améliorations

### Mode Validation guidée
- **Panneau dédié** activable depuis le tableau principal (bouton « Validation guidée »), permettant de saisir et vérifier les éléments clés d'un dossier sans quitter l'outil
- **Particulièrement recommandé pour les néocollaborateurs** et les collaborateurs présentant un taux de conformité avec une forte marge de progression : le panneau guide étape par étape la vérification de chaque document et réduit les erreurs de saisie ou d'oubli
- **Section Carte grise** : immatriculation, 1ère MEC, PAD (pas assuré depuis), puissance (P.6), date d'acquisition ; boutons toggle Nom différent, Titulaire, Cotitulaire, Leasing
- **Section Permis de conduire** : date de naissance, date d'obtention du permis ; boutons toggle Nom différent et Suspension / Annulation
- **Section Relevé d'informations** : antécédents justifiés (calculés automatiquement depuis le tableau de périodes) et déclarés, CRM justifié et CRM déclaré, résiliation, sinistralité avec alerte visuelle en cas d'écart
- **Section RIB** : gestion du titulaire, cotitulaire et des divergences de domiciliation
- **CRM suggéré → validation** : le CRM le plus récent calculé par la frise est automatiquement injecté dans le champ CRM justifié
- Bouton **Réinitialiser** pour vider le panneau en un clic

### Commentaire client automatique
- **Génération automatique** d'un commentaire structuré construit à partir des éléments cochés dans la validation guidée
- **Messages contextuels** prêts à l'envoi : un clic copie le message dans le presse-papier

### Menu principal (☰)
- **Panneau latéral** centralisé : accès à tous les outils, la validation guidée et les nouveautés en un clic
- Badge animé signalant une mise à jour disponible
- Bascule thème **clair / sombre** intégrée dans le menu

### Correctifs
- Mode sombre adouci pour un rendu plus confortable
- Persistance du mode simple / complexe après effacement

---

## v1.0 — Sauvegarde & Mode Complexe

### Mode Complexe
- Colonnes avancées : Immatriculation, Échéance, CRM dern. échéance, Sinistres, Date permis
- Alertes CRM automatiques (interruption > 24 mois, incompatibilité avec ancienneté du permis)
- **CRM suggéré** calculé en temps réel

### Sauvegarde de contrat
- Jusqu'à **1 000 contrats** sauvegardables en local avec auto-sauvegarde et protection à l'effacement

### Autres
- Format de dates flexible (JJ/MM/AAAA, JJMMAA…)
- Commentaire RI personnalisable
- Popup Paramètres
- Bouton Nouveautés avec changelog intégré

---

## v0.31 — Version de base
- Tableau de saisie + calcul CRM automatique
- Frise visuelle des périodes et interruptions
- Outils : Tableau CRM, Impact CRM, CRM max permis, Période précise, Loi Hamon
- Mode Moto (fenêtre 24 mois)
- Thème clair / sombre
