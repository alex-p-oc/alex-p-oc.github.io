# Comment déployer ce portfolio sur GitHub Pages

## 1. Personnaliser le contenu
Ouvre `index.html` et remplace :
- `Prénom Nom` par ton nom
- les liens `https://github.com/ton-pseudo` par ton vrai profil GitHub
- les 6 blocs `.project` par tes vrais projets (titre, description, lien, technos)
- `ton.email@exemple.com` et le lien LinkedIn dans la section contact
- (optionnel) ajoute un fichier `CV.pdf` à côté de `index.html` si tu veux proposer un téléchargement

## 2. Créer le repo GitHub Pages
1. Sur GitHub, crée un nouveau repo nommé **exactement** `ton-pseudo.github.io`
   (remplace `ton-pseudo` par ton nom d'utilisateur GitHub)
2. Mets `index.html` (et `CV.pdf` si tu l'ajoutes) à la racine du repo

## 3. Publier
```bash
git init
git add index.html README.md
git commit -m "Portfolio initial"
git branch -M main
git remote add origin https://github.com/ton-pseudo/ton-pseudo.github.io.git
git push -u origin main
```

Ton site sera visible en quelques minutes à l'adresse :
`https://ton-pseudo.github.io`

## 4. Mettre à jour
Chaque `git push` sur la branche `main` republie automatiquement le site,
pas besoin de configuration supplémentaire.
