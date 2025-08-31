# Carte interactive – Les 3 Vallées (OpenSnowMap / OpenStreetMap)

Cette petite app statique affiche les pistes et remontées mécaniques des **3 Vallées** via :

- **Calque de pistes OpenSnowMap** (`https://tiles.opensnowmap.org/pistes/{z}/{x}/{y}.png`).
- **Données en direct OpenStreetMap** (Overpass API) pour les remontées `aerialway=*` et stations.

## Déploiement rapide

### Option A — GitHub Pages (recommandé)
1. Créez un dépôt GitHub vide (public ou privé).
2. Uploadez `index.html` (et ce README).
3. Dans **Settings → Pages**, choisissez **Deploy from a branch**, branche `main`, dossier `/root`.
4. Patientez 1–2 min, l’URL sera du type `https://<votre-user>.github.io/<repo>/`.

### Option B — Netlify Drop
- Allez sur https://app.netlify.com/drop et glissez le dossier. Netlify fournit une URL publique.

### Option C — Vercel
- Importez le dépôt GitHub sur https://vercel.com/ → déploiement statique instantané.

## Points importants (licences/usage)
- **OpenSnowMap (tuiles)** : n’utilisez pas de **téléchargement massif**, fournissez une **attribution** et un **referer** valide. Pour des usages soutenus, préférez l’auto‑hébergement des tuiles/MBTiles. Cf. https://www.opensnowmap.org/iframes/about.eng.html
- **OpenStreetMap (fond & données)** : crédit « © OpenStreetMap contributors ». La **politique d’usage des tuiles** OSM (si vous utilisez `tile.openstreetmap.org`) impose des limites ; pour la production, vous pouvez utiliser un fournisseur tiers ou votre propre serveur. Cf. https://operations.osmfoundation.org/policies/tiles/

## Ajustements
- Modifiez la **BBOX** dans `index.html` pour élargir/réduire l’emprise.
- Ajoutez des champs supplémentaires dans les pop‑ups (ex: `aerialway:capacity`, `duration`, `operator`…).

Bon ski !
