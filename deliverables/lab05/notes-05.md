# TP5 - Notes

## Difficultes rencontrees
- Comprendre la difference entre preview et production sur Vercel.
- Configurer les secrets (token, org id, project id) au bon endroit.
- Reutiliser un artifact de build pour deployer avec vercel --prebuilt.
- Gerer les triggers (pull_request pour preview, manuel pour production).

## Ce que j ai appris
- Mettre en place un pipeline CD avec GitHub Actions et Vercel.
- Produire un artifact et le reutiliser pour le deploy.
- Deployer automatiquement en preview lors d une PR.
- Garder un deploy de production manuel avec validation humaine.
- Promouvoir un preview vers la production (blue green).
