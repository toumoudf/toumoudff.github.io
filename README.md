# Mini-site Toumoudff Games (GitHub Pages)

Rôle : héberger `app-ads.txt` à la racine d'un domaine (AdMob le vérifie sur le « site web du
développeur » déclaré dans la Play Console) et renvoyer les visiteurs vers le blog Blogger.

| Fichier | Rôle |
|---|---|
| `app-ads.txt` | la ligne du compte AdMob, valable pour toutes les apps du compte |
| `index.html` | redirige vers https://coindevtumu.blogspot.com/ |
| `.nojekyll` | GitHub sert les fichiers tels quels |

## Mise en ligne (une seule fois)

1. Sur https://github.com, connecte-toi, puis **New repository**.
2. Nom du dépôt : **`<ton-nom-github>.github.io`** (exactement ton nom d'utilisateur suivi de `.github.io`),
   **Public**, puis **Create repository**.
3. Sur la page du dépôt : **uploading an existing file** → glisse `app-ads.txt`, `index.html` et
   `.nojekyll` → **Commit changes**.
4. Attends 1 à 2 minutes, puis ouvre `https://<ton-nom-github>.github.io/app-ads.txt` : la ligne
   `google.com, pub-5891997737187580, DIRECT, f08c47fec0942fa0` doit s'afficher.

## Ensuite

1. **Play Console**, pour chaque app : Croissance › Présence sur le Store › Fiche principale (ou
   Paramètres du Store › Coordonnées) › **Site Web** = `https://<ton-nom-github>.github.io`
   (sans rien après le nom).
2. **AdMob** › Applications › chaque app › **app-ads.txt** : la vérification se fait seule, en
   général sous 24 h (parfois quelques jours), une fois l'app publiée et la fiche à jour.

Si un jour un autre réseau publicitaire te donne sa propre ligne (compte direct AppLovin,
Unity…), ajoute-la sur une nouvelle ligne de `app-ads.txt`. La médiation AdMob n'en demande pas.
