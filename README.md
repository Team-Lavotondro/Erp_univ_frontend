# ERP Universitaire — Frontend

Application frontend de gestion d'un système ERP universitaire.

Ce projet est développé avec **React, Vite, TypeScript, Tailwind CSS et shadcn/ui**.

##  Technologies

* React
* Vite
* TypeScript
* Tailwind CSS
* shadcn/ui
* React Router
* Lucide React
* ESLint

##  Structure du projet

```text
src/
├── assets/
│   └── index.css
│
├── components/
│   ├── layout/
│   │   ├── AdminLayout.tsx
│   │   ├── Header.tsx
│   │   └── Sidebar.tsx
│   │
│   └── ui/
│       ├── button.tsx
│       ├── input.tsx
│       ├── card.tsx
│       └── ...
│
├── pages/
│   ├── Login.tsx
│   ├── Dashboard.tsx
│   ├── Users.tsx
│   └── Settings.tsx
│
├── routes/
│   └── AppRoutes.tsx
│
├── lib/
│   └── utils.ts
│
├── App.tsx
└── main.tsx

components.json
package.json
tsconfig.app.json
tsconfig.node.json
vite.config.ts
```

##  Installation

Cloner le repository :

```bash
git clone <URL_DU_REPOSITORY>
```

Entrer dans le projet :

```bash
cd erp-univ-front
```

Installer les dépendances :

```bash
npm install
```

##  Lancer le projet

Démarrer le serveur de développement :

```bash
npm run dev
```

L'application sera disponible sur :

```text
http://localhost:5173
```

##  Build

Pour créer la version de production :

```bash
npm run build
```

Pour vérifier la version buildée :

```bash
npm run preview
```

##  shadcn/ui

Les composants shadcn/ui sont stockés directement dans le projet.

Par exemple :

```text
src/components/ui/button.tsx
```

Pour ajouter un nouveau composant :

```bash
npx shadcn@latest add button
```

Exemple d'utilisation :

```tsx
import { Button } from "@/components/ui/button"

export default function Example() {
  return (
    <Button>
      Ajouter
    </Button>
  )
}
```

##  Tailwind CSS

Tailwind CSS permet de construire l'interface directement avec les classes CSS.

Exemple :

```tsx
<div className="flex items-center justify-between p-4">
  <h1 className="text-2xl font-bold">
    Dashboard
  </h1>

  <Button>
    Ajouter
  </Button>
</div>
```

##  Routes

Les principales routes de l'application sont organisées avec React Router.

```text
/login
/admin
/admin/users
/admin/settings
```

##  Développement en équipe

Avant de commencer à travailler :

```bash
git pull origin main
```

Créer une branche pour votre fonctionnalité :

```bash
git checkout -b feature/nom-fonctionnalite
```

Après avoir terminé :

```bash
git add .
git commit -m "feat: ajouter gestion des utilisateurs"
git push origin feature/nom-fonctionnalite
```

Ensuite, créer une **Pull Request** vers `main`.

### Convention des commits

Nous utilisons des messages de commit simples et explicites :

```text
feat: nouvelle fonctionnalité
fix: correction d'un bug
refactor: amélioration du code
style: modification du style
docs: modification de la documentation
chore: configuration ou dépendances
```

Exemples :

```bash
git commit -m "feat: ajouter page dashboard"
git commit -m "fix: corriger formulaire de connexion"
git commit -m "style: améliorer sidebar"
```

##  Règles de développement

* Ne pas travailler directement sur `main`.
* Créer une branche pour chaque fonctionnalité.
* Faire des commits clairs.
* Tester le projet avant de faire une Pull Request.
* Ne pas pousser les fichiers `.env`.
* Respecter la structure du projet.
* Réutiliser les composants shadcn/ui lorsque cela est possible.

##  Variables d'environnement

Les variables sensibles doivent être placées dans un fichier `.env`.

Exemple :

```env
VITE_API_URL=http://localhost:3000
```

Ne jamais pousser le fichier `.env` sur GitHub.

Utiliser plutôt :

```text
.env.example
```

Exemple :

```env
VITE_API_URL=
```

##  Licence

Projet team Lavotondro — EMIT / Université de Fianarantsoa.

