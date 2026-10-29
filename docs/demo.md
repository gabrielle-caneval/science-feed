# Démonstration Science Feed

Enregistrement du 29 octobre 2026, environ 31 secondes, application locale compilée avec `npm run build` puis lancée avec `npm start`.

La vidéo montre le choix IA & Machine Learning, le flux, la sauvegarde d’un article et sa présence dans la bibliothèque, puis une recherche « graph neural networks » qui a renvoyé 15 résultats réels pendant la capture. Le compte est un compte local de test. Le flux est préparé avec refillInterest, via les connecteurs arXiv et Semantic Scholar du projet ; aucune réponse API n’est simulée. La disponibilité et les quotas des sources peuvent faire varier les résultats.

La capture Chrome/Playwright ajoute un panneau explicatif à côté de l’application. Les interactions passent par son interface réelle. Vidéo muette en MP4 H.264, 1440 × 1000, explications visuelles et sous-titres français disponibles sur le portfolio.

## Vérification

Le parcours a été exécuté avec succès, sans exception JavaScript détectée dans la page. Les états résultant des actions ont été vérifiés. Cette vérification porte sur le parcours filmé ; elle ne constitue pas une couverture de toutes les fonctionnalités.

## Rejouer le parcours

Installer les dépendances et suivre le README pour le lancement. Utiliser un profil/compte de test et des données fictives. Refaire les étapes décrites ci-dessus dans l’interface. Les secrets, la session du compte de test et la base locale ne sont pas publiés.

## Correction nécessaire au lancement compilé

L’adaptateur Prisma et better-sqlite3 sont déclarés dans `serverExternalPackages` afin que Node charge le module natif SQLite au lieu d’un paquet embarqué par Webpack. Après correction : compilation, création de compte, authentification, choix d’intérêt, flux, sauvegarde et recherche vérifiés sur le serveur de production local.
