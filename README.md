# Reset CSS Alsacréations

Le fichier CSS [`reset.css`](public/reset.css) est une base de travail moderne qui uniformise l'affichage des éléments HTML entre les navigateurs tout en appliquant des bonnes pratiques d'accessibilité et en optimisant l'expérience utilisateur.

## Principales sections couvertes

- **Configuration globale** : Color-scheme et modèle de boîte
- **Éléments de base** : Styles fondamentaux pour HTML et body
- **Navigation et focus** : Gestion accessible du focus et des interactions clavier
- **Typographie** : Optimisations pour les titres, paragraphes et guillemets français
- **Listes** : Reset accessible des listes avec role="list"
- **Éléments média** : Prévention des débordements et affichage optimal
- **Formulaires** : Normalisation complète des champs et boutons
- **Éléments préformatés** : Configuration optimale pour le code
- **SVG** : Gestion moderne des graphiques vectoriels
- **Accessibilité ARIA** : Support des attributs et états ARIA
- **Masquage accessible** : Classe `.visually-hidden` pour les lecteurs d'écran
- **Préférences utilisateur** : Respect du `prefers-reduced-motion`
- **Reset print** : Styles optimisés pour l'impression

## Utilisation

Placez ce reset dans un layer CSS `reset` sous vos autres layers pour une meilleure organisation du code.

## Méthodologie globale

Le fichier `app.css` charge toutes les feuilles de styles dans l'ordre des layers CSS :

1. **Layer reset** :

   - `reset.css` - Reset CSS moderne (et reset print)
   - `alsa-layouts.css` - Utilitaires de disposition des composants

2. **Layer theme** :

   - `theme.css` - Thème principal (valeurs primitives)
   - `theme-tokens.css` - Variables sous forme de tokens

3. **Layer components** :

   - `styles.css` - Styles globaux du projet (gabarits, typographie, etc.)
   - tous les fichiers CSS des composants (bouton, input, etc.)

4. **Layer utilities** :
   - Fichier de classes utilitaires si nécessaire (accessibilité, alignement, etc.)
