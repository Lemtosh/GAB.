# Changelog — GAB. Guide Antécédents Bonus-Malus

## v1.1 — Validation guidée, Menu principal & améliorations

### Mode Validation guidée
- **Panneau dédié** activable depuis le tableau principal (bouton "Validation guidée"), permettant de saisir et vérifier les éléments clés d'un dossier sans quitter l'outil
- **Particulièrement recommandé pour les néocollaborateurs** et les collaborateurs présentant un taux de conformité avec une forte marge de progression : le panneau guide étape par étape la vérification de chaque document et réduit les erreurs de saisie ou d'oubli
- **Section Carte grise** : immatriculation, 1ère MEC, PAD (pas assuré depuis), puissance (P.6), date d'acquisition ; boutons toggle Nom différent, Titulaire, Cotitulaire, Leasing
- **Section Permis de conduire** : date de naissance, date d'obtention du permis ; boutons toggle Nom différent et Suspension / Annulation
- **Section Relevé d'informations** : antécédents justifiés (calculés automatiquement depuis le tableau de périodes) et déclarés, CRM justifié et CRM déclaré, résiliation, sinistralité avec alerte visuelle en cas d'écart
- **Section RIB** : gestion du titulaire, cotitulaire et des divergences de domiciliation
- **Mode Supp. / Finaux** sur le champ antécédents : bascule selon le type de demande (RI supplémentaire ou relevé final)
- **Date permis synchronisée** : la date d'obtention saisie dans la validation guidée est automatiquement reportée dans toutes les cases « Date permis » du tableau complexe
- **CRM suggéré → validation** : le CRM le plus récent calculé par la frise (≤ aujourd'hui) est automatiquement injecté dans le champ CRM justifié de la validation guidée
- Bouton **Réinitialiser** pour vider le panneau en un clic

### Commentaire client automatique
- **Génération automatique** d'un commentaire structuré (partie « demande » et partie « modification ») construit en temps réel à partir des éléments cochés et saisis dans le panneau de validation
- **Messages contextuels** prêts à l'envoi (Titulaire CG, Cotitulaire, Nom différent, RI supplémentaire, divergence RIB…) : un clic sur un bouton copie le message directement dans le presse-papier

### Menu principal (☰)
- **Bouton menu fixe** (☰) en haut à gauche, remplaçant les anciens boutons flottants en bas d'écran
- **Panneau latéral** centralisé donnant accès en un clic à tous les outils (Tableau CRM, Impact CRM, CRM max permis, Période précise, Loi Hamon), à la Validation guidée et aux Nouveautés
- Badge animé sur le bouton menu signalant une mise à jour disponible
- Bascule thème **clair / sombre** intégrée directement dans le menu

### Correctifs & améliorations
- **Mode sombre adouci** : les fonds étaient jugés trop sombres ; les couleurs de fond ont été légèrement rehaussées pour un rendu plus confortable sans altérer les contrastes
- **Persistance du mode après Effacer** : le mode simple / complexe est désormais conservé après un effacement et une fermeture du navigateur. La protection contre l'effacement d'un contrat non sauvegardé reste inchangée

---

## v1.0 — Sauvegarde & Mode Complexe

### Mode Complexe
- **Switch Simple / Complexe** dans la barre principale pour activer les colonnes avancées
- **Colonne Immatriculation** : saisie de la plaque du véhicule par ligne, affichée sur la frise avec une couleur propre
- **Colonne Échéance** : date d'échéance du contrat (format JJMM), repère visuel sur la frise à chaque anniversaire
- **Colonne CRM dern. échéance** : CRM constaté à la dernière échéance, sert au calcul du CRM suggéré
- **Colonne Sinistres** : popup dédiée par ligne pour ajouter/supprimer des sinistres (type BDG, 0 %, 50 %, 100 %, Autre + date facultative)
- **Colonne Date permis** : saisie de la date de permis ligne par ligne
- **Frise agrandie** : canvas 220 px en mode complexe, repères sinistres colorés et CRM suggéré calculé

### Garde-fous du Mode Complexe
- **Alerte CRM interruption** : avertissement si une interruption dépasse 24 mois (triangle rouge, popup explicative avec les dates exactes)
- **Alerte CRM permis** : détection automatique d'un CRM saisi incompatible avec l'ancienneté du permis, détail ligne par ligne
- **CRM suggéré** : calcul en temps réel du CRM attendu à la prochaine échéance (sinistres dans fenêtre réglementaire, bonus annuel ×0,95, plafond permis)
- **Plafond 3,50 / plancher 0,50** : limites CRM strictes appliquées à chaque calcul

### Sauvegarde de contrat
- Champ **N° contrat** + bouton de sauvegarde pour sauvegarder et recharger un dossier complet (toutes les lignes, date d'effet, mode, sinistres, notes…)
- **Auto-sauvegarde** : enregistrement silencieux 5 secondes après la dernière frappe si un N° contrat est renseigné
- **Protection à l'effacement** : si des modifications non sauvegardées existent, popup de confirmation avec trois choix — Enregistrer d'abord / Effacer quand même / Annuler
- Jusqu'à **1 000 contrats** sauvegardables en local

### Autres nouveautés
- **Format de date flexible** : toutes les dates acceptent JJ/MM/AAAA, JJ-MM-AAAA, JJMMAA, etc. avec auto-correction à la sortie du champ
- **Commentaire RI personnalisable** : modèle éditable, seuil d'interruptions courtes à ignorer, option ignorer la dernière période
- **Popup Paramètres** : activation / désactivation de la sauvegarde de contrat et de l'auto-sauvegarde, sous-section extensible
- **Bouton Nouveautés** : accès à ce changelog version par version, avec badge animé lors de chaque mise à jour

---

## v0.31 — Version de base
- Tableau de saisie des antécédents avec calcul CRM automatique
- Frise visuelle des périodes couvertes et des interruptions
- **Outils** : tableau CRM standard, calculateur Impact CRM (sinistres 0 % / 50 % / 100 %), CRM maximum selon date de permis
- **Outils** : calcul d'une période précise, outil Loi Hamon
- Mode **Moto** : fenêtre de 24 mois
- Thème clair / sombre
- Détection automatique de mise à jour avec bannière de rechargement
