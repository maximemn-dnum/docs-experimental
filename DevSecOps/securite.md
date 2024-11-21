# Sécurité

## Gestion des secrets

### Checklist

- [ ] utiliser des variables d'environnement pour configurer les secrets de l'application
- [ ] ne pas inclure de secrets non chiffrés dans le code source
- [ ] utiliser l'outil talisman (ou équivalent) dans un pre-commit hook git
- [ ] ne pas inclure de secrets non chiffrés dans les images docker
  - par ex : le token Sentry pour pousser les source maps 
- [ ] ne pas afficher les secrets dans les logs ni les envoyer sur sentry
- [ ] utiliser les outils à disposition pour les projets open source
  - ex : GitGuardian


## Anonymisation des données

### Checklist

- [ ] générer un dump anonymisé de la DB 
  - pour recharger en environnement d'intégration/preprod
  - pour calculer des KPI
