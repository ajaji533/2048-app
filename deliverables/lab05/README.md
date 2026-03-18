# Lab05 - CD Vercel (GitHub Actions)

## Secrets GitHub
Ajoute ces secrets dans le repo GitHub:
- Settings -> Secrets and variables -> Actions -> New repository secret
- VERCEL_TOKEN
- VERCEL_ORG_ID
- VERCEL_PROJECT_ID

## Tester le preview (PR vers lab05)
1) Cree une branche et ouvre une Pull Request vers lab05.
2) Le job preview_deploy s execute.
3) Ouvre les logs du job pour recuperer l URL preview fournie par Vercel.

## Tester la production (manuel)
1) Onglet Actions -> workflow "Lab05 Vercel CD".
2) Clique Run workflow (workflow_dispatch).
3) Le job production_deploy s execute et deploie en production.

## Promote to production (blue-green)
Depuis le dashboard Vercel:
1) Ouvre le projet et choisis un deployment preview.
2) Clique Promote to Production pour basculer la version en production.
