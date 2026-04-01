# Conclusion

Le preview Vercel permet de valider une version pour chaque PR, tandis que la production sert la version officielle aux utilisateurs. Le blue-green deployment via "Promote to Production" permet de publier une version deja construite sans coupure et avec un retour arriere possible. GitHub Actions orchestre le pipeline: build, creation d'artifact, deploiement preview automatique et deploiement production manuel avec validation humaine via l'environnement "production".
