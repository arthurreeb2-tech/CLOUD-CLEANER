# Cloud Cleaner

Fait de la place dans iCloud Drive, Google Drive et OneDrive depuis un Mac, sans risque.

**Page et téléchargement : https://arthurreeb2-tech.github.io/CLOUD-CLEANER/**

Ce dépôt sert à distribuer l'app et ses mises à jour (GitHub Pages) :

| Fichier | Rôle |
|---|---|
| `index.html` | Page de présentation et de téléchargement |
| `Cloud-Cleaner-Mac.zip` | App complète, pour une première installation |
| `version.json` | Dernière version : empreinte SHA-256 et signature Ed25519 |
| `maj/cloudcleaner-<version>.zip` | Paquets de mise à jour (les 3 derniers) |
| `historique.json` | Liste des versions publiées |

L'app vérifie `version.json` à chaque lancement. Elle n'accepte un paquet que si sa signature
correspond à la clé publique intégrée à l'app et si son empreinte est exacte. Elle l'installe au
lancement suivant, et revient à la version précédente si la nouvelle ne démarre pas.

Fichiers générés par `scripts/publier-maj.py` : ne pas les modifier à la main.
