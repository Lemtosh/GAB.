# Changelog — GAB. Guide Antécédents Bonus-Malus

## v0.32 — Sauvegarde & Mode Complexe

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
