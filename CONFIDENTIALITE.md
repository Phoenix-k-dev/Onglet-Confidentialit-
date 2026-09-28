# Politique de confidentialité — Onglet+

*Dernière mise à jour : 27 septembre 2026*

Onglet+ est une extension pour Microsoft Edge qui remplace la page « Nouvel onglet ». Cette page explique quelles données l'extension utilise.

## En résumé

- **Pas de compte, pas de publicité, pas de statistiques, pas de revente de données.**
- Tes raccourcis, pages, notes, tâches et réglages sont enregistrés **uniquement dans ton navigateur** (`chrome.storage.local` et IndexedDB).
- Le développeur n'a **aucun serveur** et ne reçoit **aucune donnée**.

## Données enregistrées sur ton appareil

| Donnée | Où | Pourquoi |
|---|---|---|
| Raccourcis, pages, dossiers, dock, réglages, notes, tâches | Stockage local de l'extension | Faire fonctionner la page Nouvel onglet |
| Image de fond importée | IndexedDB (local) | Afficher ton fond d'écran |
| Cache des icônes et de la météo | localStorage (local) | Accélérer l'affichage |

Si tu utilises **« Sauvegarder dans le cloud »**, une copie compressée de ces données est placée dans `chrome.storage.sync`. C'est Microsoft Edge qui la synchronise avec ton propre compte Microsoft, si la synchronisation est activée. Le développeur n'y a pas accès.

## Services externes contactés

L'extension contacte des services tiers uniquement pour les fonctions suivantes :

| Service | Quand | Informations envoyées |
|---|---|---|
| Google (`www.google.com/s2/favicons`) puis DuckDuckGo (`icons.duckduckgo.com`) | Affichage des icônes des sites (option « Icônes des sites : En ligne », désactivable) | Le nom de domaine du raccourci (ex. `github.com`) |
| Open-Meteo (`api.open-meteo.com`, `geocoding-api.open-meteo.com`) | Widget Météo (désactivable) | Les coordonnées de la ville choisie, ou le texte tapé pour rechercher une ville |
| Bing (`www.bing.com`) | Uniquement si tu choisis « Image Bing du jour » | Une requête pour obtenir l'image du jour |
| Les sites de tes favoris | Uniquement quand tu cliques sur « Chercher les liens morts » | Une simple requête sans cookies vers chaque favori du dossier choisi, pour savoir s'il répond |
| Le moteur de recherche que tu choisis | Quand tu lances une recherche | Le texte de ta recherche |

Ces services ont leurs propres politiques de confidentialité. L'extension ne leur transmet aucun identifiant personnel.

## Permissions

- **storage** : enregistrer tes données localement.
- **activeTab** : quand tu cliques sur le bouton Onglet+, lire le titre et l'adresse de l'onglet actif pour l'ajouter en raccourci.
- **search** : lancer une recherche avec le moteur par défaut d'Edge.
- **history** *(facultative, demandée au clic)* : classer tes sites les plus visités et repérer les favoris jamais
  ouverts. L'historique est lu **sur ton appareil uniquement** et n'est jamais envoyé.
- **bookmarks** *(facultative, demandée au clic)* : importer un dossier de favoris et l'outil « Nettoyer mes favoris ».
  Tes favoris ne sont supprimés ou renommés **qu'après une action de ta part** (confirmation, ou option de
  synchronisation que tu actives), et chaque suppression peut être annulée.
- **www.bing.com** *(facultative, demandée au clic)* : récupérer l'image Bing du jour.

## Suppression des données

Désinstaller l'extension supprime toutes ses données locales. Tu peux aussi utiliser **Paramètres → Données → Tout réinitialiser**.

## Contact

Pour toute question, ouvre une *issue* sur le dépôt GitHub du projet.

---

# Privacy policy — Onglet+ (English)

Onglet+ replaces the Microsoft Edge New Tab page. **No account, no ads, no analytics, no data sale.** All shortcuts, notes, tasks and settings are stored locally in your browser. The developer runs no server and receives no data.

External services are contacted only for these features: site icons (Google/DuckDuckGo receive the shortcut's domain name; can be turned off), weather (Open-Meteo receives the chosen city's coordinates or your city search text), the optional Bing image of the day (bing.com), the search engine you choose (receives your search text), and, only when you click "Look for dead links", each favorite of the chosen folder (a cookie-less request to check it responds). Optional permissions: history (ranks your most visited sites and finds never-opened favorites, read locally, never sent) and bookmarks (import, and cleanup; favorites are only deleted or renamed after an explicit action, and every deletion can be undone). The optional "cloud backup" stores a compressed copy in `chrome.storage.sync`, which Edge syncs with your own Microsoft account.

Uninstalling the extension deletes all its local data.
