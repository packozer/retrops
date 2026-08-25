# Post-its — Rétrospectives d'équipe

Outil léger de rétrospective en temps réel. Chaque participant rejoint la salle depuis son navigateur avec un code à 5 caractères.

## Fonctionnalités

- **4 templates de rétro** : Start/Stop/Continue, Mad/Sad/Glad, 4 L's, Sailboat
- **Post-its collaboratifs** : ajout, drag & drop, vote ❤
- **Plan d'action** : transformer un post-it en tâche assignable
- **Timer partagé** : 5, 10 ou 15 min visible par tous
- **Export Markdown** : copier la rétro en un clic

## Déploiement

### Vercel (recommandé)

```bash
npm i -g vercel
vercel
```

### Local

```bash
npx serve public -l 3000
```

Puis ouvrir http://localhost:3000

## Stack

Zero dépendance — un seul fichier HTML avec CSS et JS vanilla.
La synchronisation multi-utilisateurs repose sur le localStorage partagé de l'artifact Claude. Pour un déploiement en production, remplacer par un backend WebSocket + base de données (Firebase, Supabase, etc.).

## Licence

MIT
