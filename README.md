# Site vitrine CARSAJ

Site statique premium en français pour CARSAJ, société casablancaise dont l'activité déclarée comprend l'extraction et l'exploitation de matériaux, notamment le sable naturel pour la construction.

## Structure

- `index.html` : accueil, activités, processus, identité et FAQ
- `about.html` : profil et identité de l'entreprise
- `services.html` : détail fidèle des activités déclarées
- `contact.html` : adresse et identifiants officiels
- `privacy-policy.html` : politique adaptée au fonctionnement réel du site
- `404.html` : page d'erreur
- `assets/css/` : design, animations et responsive
- `assets/js/` : navigation, défilement et animations
- `assets/icons/favicon.svg` : favicon/monogramme CSS-SVG temporaire
- `robots.txt` et `sitemap.xml` : bases SEO à finaliser avec le domaine

## Ouvrir localement

Ouvrez `index.html` directement, ou lancez un serveur dans ce dossier :

```powershell
python -m http.server 8000
```

Puis ouvrez `http://localhost:8000`.

## Personnalisation

- Informations société : recherchez `CARSAJ`, `003659686000050`, `657053` et l'adresse dans les fichiers HTML.
- Logo : remplacez le composant `.brand` dans chaque page et `assets/icons/favicon.svg` après réception du logo officiel.
- Images : créez `assets/images/`, utilisez des noms descriptifs, `loading="lazy"`, des dimensions explicites et des formats WebP/AVIF.
- Couleurs : modifiez les variables au début de `assets/css/style.css`.
- Activités : modifiez les cartes de `index.html` et les blocs de `services.html` uniquement avec des informations validées.
- SEO : remplacez les métadonnées page par page et ajoutez les URL Open Graph définitives.
- Sitemap : remplacez toutes les occurrences de `https://example.com` dans `sitemap.xml` et `robots.txt`.

## Contact et formulaire

Aucun e-mail, téléphone ou WhatsApp officiel n'a été fourni. Le site n'affiche donc pas de formulaire factice et ne prétend pas transmettre de message. Après validation des coordonnées, ajoutez les liens `mailto:`/`tel:`/WhatsApp. Pour un formulaire, connectez un endpoint serveur sécurisé, affichez les états d'erreur et de succès réels, ajoutez le consentement avec un lien vers `privacy-policy.html`, et mettez à jour la politique.

## Confidentialité et cookies

Le site n'utilise actuellement aucun cookie, stockage local, outil d'analyse, police externe, carte embarquée ou formulaire. Aucun bandeau cookie n'est donc nécessaire. Le lien OpenStreetMap est externe et s'ouvre à la demande. Si des outils non essentiels sont ajoutés, bloquez leur chargement avant consentement, fournissez Accepter/Refuser et permettez de modifier le choix. Mettez alors à jour la politique.

La politique est un projet adapté à cette version technique du site. Elle doit être examinée par un professionnel qualifié avant publication. L'hébergeur, ses journaux techniques et leurs durées de conservation devront y être ajoutés.

## Sécurité et déploiement

Le projet n'emploie aucune dépendance ni secret. En production, servir en HTTPS et définir une Content Security Policy restrictive, par exemple `default-src 'self'; img-src 'self' data:; style-src 'self'; script-src 'self'; base-uri 'self'; form-action 'self'`. La page de confidentialité contient actuellement un petit gestionnaire `onclick` pour l'impression ; remplacez-le par un écouteur dans `main.js` si cette CSP est appliquée sans `'unsafe-inline'`.

- GitHub Pages : pousser le dossier dans un dépôt, puis activer Pages sur la branche principale.
- Netlify : glisser le dossier dans Netlify Drop ou connecter le dépôt ; aucun build n'est requis.
- Vercel : importer le dépôt comme site statique, sans commande de build.
- Hébergement classique : transférer tous les fichiers en conservant l'arborescence.

## Information required before production launch

- [ ] Domaine de production
- [ ] Logo officiel et éventuelles règles de marque
- [ ] Téléphone professionnel validé
- [ ] Adresse e-mail professionnelle
- [ ] Numéro WhatsApp officiel, si utilisé
- [ ] Adresse e-mail ou canal pour les demandes de confidentialité
- [ ] Confirmation de l'écriture complète de la raison sociale
- [ ] Nom du représentant légal, seulement s'il doit être publié
- [ ] Horaires d'ouverture
- [ ] Description détaillée et validée des prestations
- [ ] Sites d'exploitation, zones desservies et certifications éventuelles
- [ ] Photos dont CARSAJ détient les droits
- [ ] Hébergeur et politique de journaux techniques
- [ ] Backend du formulaire, si un formulaire est souhaité
- [ ] Choix analytique et exigences cookies, si une mesure d'audience est souhaitée
- [ ] Relecture juridique de la politique de confidentialité
- [ ] URL d'image Open Graph

## Sources et hypothèses

Les données publiques proviennent exclusivement des fichiers fournis : document fiscal `CARSAJ_952310200.docx`, `merged_data.json`, `directinfo_data.json`, données DUNS et rapport de vérification. Le secteur « Automotive » présent dans une source DUNS n'a pas été retenu car il contredit l'activité détaillée du document fiscal. Aucun chiffre de performance, témoignage, prix, certification ou engagement environnemental n'a été inventé. Le mot « matériaux » du logo textuel est une signature éditoriale temporaire, pas une modification de la raison sociale.
