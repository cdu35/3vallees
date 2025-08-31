# 3 Vallées – Carte (cache GeoJSON) + MapLibre

Deux front‑ends :
- `index.html` (Leaflet raster + overlay OpenSnowMap) – lit uniquement `data/remontees_3vallees.geojson`.
- `index-maplibre.html` (MapLibre GL vector + OpenFreeMap + overlay OpenSnowMap) – lit le même cache.

## Déploiement GitHub Pages
1. Pousser ces fichiers sur `main`.
2. **Settings → Pages** → Deploy from a branch → `main` / `/root`.
3. Ouvrir `…/index.html` ou `…/index-maplibre.html`.

## Mettre à jour le cache (Overpass → GeoJSON)
- **Actions → Build cached GeoJSON (3 Vallées) → Run workflow** (ou attendre la planification chaque lundi 03:00 UTC).

## Licences
- OpenStreetMap (ODbL) – © Contributors
- OpenSnowMap tiles (pistes) – CC‑BY‑SA, referer valide, pas de bulk download
