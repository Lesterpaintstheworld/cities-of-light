## Choix Technologiques - Cartographie

### Mapbox GL JS

Pour la composante cartographique centrale de l'interface utilisateur, nous utiliserons Mapbox GL JS avec les motivations suivantes :

#### Avantages Techniques
- Rendu vectoriel performant via WebGL
- Support natif des cartes 3D et de l'extrusion des bâtiments
- Intégration React native via react-map-gl
- Gestion optimisée des données géospatiales (GeoJSON, Vector Tiles)
- API complète pour la personnalisation des styles et interactions
- Support des modèles 3D personnalisés
- Système de contrôles extensible

#### Intégration Projet
- Compatible avec notre stack React/Three.js
- Permet l'ajout progressif de fonctionnalités 3D
- Excellente documentation et exemples
- Communauté active et support professionnel disponible
- Pricing flexible selon l'usage

#### Alternatives Considérées
- Leaflet : Plus léger mais limité en 3D
- Google Maps : Moins flexible pour la personnalisation
- OpenLayers : Courbe d'apprentissage plus raide

#### Prochaines Étapes
1. Mise en place d'un POC avec react-map-gl
   - Configuration du token Mapbox dans .env
   - Création du composant Map de base
   - Définition du style initial de la carte
2. Tests de performance avec différents volumes de données
3. Définition des styles de carte personnalisés
4. Exploration des intégrations Three.js

#### Configuration
Pour utiliser Mapbox GL JS, un token d'accès est requis :
1. Créer un compte sur mapbox.com
2. Générer un token public (default public token)
3. Stocker le token dans .env.local :
   ```
   REACT_APP_MAPBOX_TOKEN=votre_token_ici
   ```
