# Intégration continue (CI)

L'intégration continue est la pratique de contrôle qualité automatique de l'application, effectuée typiquement à chaque commit ou pull/merge request.

## Checklist

La CI doit inclure :

- [ ] les tests (unitaires, intégration, end-to-end)
  - Attention particulière portée à la partie API et authentification
  - Avoir un scenario complet "standard" en test end-to-end
  - Inclure des tests d'accessibilité pour le frontend
  - Ajouter un test lighthouse pour le frontend 
    - notamment pour l'accessibilité, le test doit être à 100%
- [ ] le formatage du code (ex: prettier en js)
- [ ] qualité de code (analyse statique du code)
  - [ ] linter
  - [ ] SonarQube
      - code smells
      - duplication
      - complexité 
      - security hotspots
- [ ] mises à jour régulières des dépendances
  - systématiquement pour les versions mineures
  - attention aux failles de sécurité
  - utilisation d'un outil supplémentaire en fonction de l'écosystème (par ex SocketSecurity dans le monde javascript) pour vérifier les vulnérabilités des dépendances utilisées.
