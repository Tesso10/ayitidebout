# Ayiti Debout — MVP Phase 1

Application Next.js — module « Konprann Vòt Mwen », 3 istwa, mode visiteur, sans authentification.

## Contenu

- `data/situations.ts` — le texte des 3 istwa. Toute modification de contenu se fait ici, un seul fichier.
- `public/audio/` — les 3 enregistrements audio réels (2 voix).
- `components/IstwaFlow.tsx` — la logique d'interaction (scène → fierté nationale → question → feedback).

## Déployer sans terminal (guide pas-à-pas)

Tu n'as pas besoin de Claude Code ni d'installer quoi que ce soit sur ton Mac. Tout se fait dans le navigateur.

### 1. Créer un compte GitHub (si pas déjà fait)
Va sur github.com → Sign up → gratuit.

### 2. Créer un nouveau dépôt (repository)
- Clique sur le bouton vert **"New"**
- Nom : `ayiti-debout`
- Laisse "Public" ou choisis "Private"
- Ne coche aucune case (pas de README, pas de .gitignore — on les a déjà)
- Clique **"Create repository"**

### 3. Uploader les fichiers
- Sur la page du dépôt vide, clique **"uploading an existing file"**
- Glisse-dépose TOUT le contenu de ce dossier (tous les fichiers et sous-dossiers)
- En bas, clique **"Commit changes"**

### 4. Déployer sur Vercel
- Va sur vercel.com → **"Sign up"** → choisis **"Continue with GitHub"**
- Une fois connecté, clique **"Add New..." → "Project"**
- Trouve `ayiti-debout` dans la liste → clique **"Import"**
- Laisse tous les réglages par défaut → clique **"Deploy"**
- Après 1-2 minutes, tu as un lien en ligne (ex. `ayiti-debout.vercel.app`) — c'est ton application, accessible à tout le monde.

### 5. (Optionnel) Analytics
Pour activer le suivi de complétion/retour (Plausible) :
- Crée un compte sur plausible.io (période d'essai gratuite, ou alternative gratuite : umami.is)
- Ajoute ton domaine (celui donné par Vercel)
- Dans Vercel : Project → Settings → Environment Variables → ajoute `NEXT_PUBLIC_PLAUSIBLE_DOMAIN` avec ton domaine comme valeur
- Redéploie (Vercel → Deployments → "..." → Redeploy)

## Pour la suite (modifications)

Reviens dans cette conversation avec Claude, décris ce que tu veux changer, et Claude régénère les fichiers concernés. Tu re-uploades juste les fichiers modifiés sur GitHub (glisser-déposer par-dessus les anciens, GitHub Web permet ça directement dans le dossier concerné) — Vercel redéploie automatiquement à chaque changement.
