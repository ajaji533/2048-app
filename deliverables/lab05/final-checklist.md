# Lab05 - Final checklist

## Ce qui est deja valide
- Build + artifact cree par GitHub Actions (job `build`).
- Preview deploy auto lors d'une pull request vers `lab5` (job `preview_deploy`).
- Deploiement production manuel via `workflow_dispatch` (job `production_deploy`).
- Secrets GitHub reutilises pour Vercel (`VERCEL_TOKEN`, `VERCEL_ORG_ID`, `VERCEL_PROJECT_ID`).
- Modification visible "MY SCORE" presente sur le preview et en production.

## Blue-green deployment dans Vercel (Promote to Production)
1) Ouvrir Vercel > Project > Deployments.
2) Trouver le dernier deployment de preview (branche `lab5` ou PR).
3) Ouvrir le menu du deployment et choisir "Promote to Production".
4) Confirmer. Vercel promeut ce build comme production sans rebuild.

## Verifier que l'URL production sert la nouvelle version
- Ouvrir l'URL de production dans une fenetre privee.
- Verifier le texte visible ("MY SCORE") ou un marqueur visuel unique.
- Optionnel: verifier l'horodatage ou l'ID du deployment en haut de la page Vercel.

## Verifier que l'ancienne version n'est plus exposee
- Recharger l'URL production en mode prive, sans cache.
- Comparer avec l'ancien deployment dans Vercel: il reste en historique mais n'est plus "Production".
- Verifier que l'ancienne version n'apparait plus sur l'URL production.

## Captures d'ecran a garder
- GitHub Actions: pipeline vert avec jobs `build`, `preview_deploy`, `production_deploy`.
- Vercel Deployments: preview avec bouton "Promote to Production".
- Vercel Deployments: deployment marque "Production" apres promotion.
- URL de production affichant "MY SCORE".
- Eventuellement: historique montrant que l'ancien deployment n'est plus "Production".
