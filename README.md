# TrueFoam GUI — CFD de drones FPV sur PC (TalkTrueFPV)

Calcul de l'écoulement de l'air autour d'un drone FPV à partir de son STL, sur votre PC Windows, avec
**OpenFOAM v2412** : traînée (S·Cx), portance, carte de pression, coupes de vitesse, lignes de courant, souffle des
hélices, régime instationnaire. Gratuit, hors ligne, sans ligne de commande.

TrueFoam GUI ouvre aussi les calculs faits sur le calculateur en ligne **TALKTRUE FPV V4** (zip « Écoulement »
ou « Dossier d'étude ») : à la place de ParaView, ou en plus.

## ⬇️ Télécharger

**[TrueFOAM-Windows.zip (dernière version)](https://github.com/Jschmiedd/TrueFoam-GUI/releases/latest/download/TrueFOAM-Windows.zip)**

Toutes les versions : [Releases](https://github.com/Jschmiedd/TrueFoam-GUI/releases).

## Installer

1. **Docker Desktop** ([docker.com](https://www.docker.com/products/docker-desktop/), option WSL 2), lancé :
   « Engine running ».
2. Une fois, dans PowerShell : `docker pull opencfd/openfoam-default:2412`
3. Dézipper **TrueFOAM-Windows.zip**, lancer **TrueFOAM.exe** (logiciel non signé : « Informations
   complémentaires » > « Exécuter quand même »). Raccourcis bureau et menu Démarrer créés au premier lancement.
4. Ruban **Exécuter** : bouton du moteur orange → cliquer une fois (1 à 5 min) ; il passe au vert « Moteur prêt ».

Détails : `LISEZMOI.txt` dans le zip.

## Ce que fait TrueFoam GUI

| | |
|---|---|
| Étude | STL (mm, cm, m, pouce), orientation, attitude de vol, vitesse, inclinaisons, air (altitude, température) |
| Physique | k-ω SST, Spalart-Allmaras, k-ε réalisable, k-ε, laminaire ; stationnaire ou instationnaire ; souffle des hélices |
| Maillage | automatique ou niveaux imposés, couches limites, étude d'indépendance au maillage ; domaine automatique, préréglé ou sur mesure, contrôle d'obstruction |
| Calcul | nombre de cœurs au choix, état du moteur en couleur, journal en direct |
| Résultats | S·Cx, Cx, forces en N, convergence, pression Cp, coupes (vitesse, pression), sonde au clic, lignes de courant 3D, frottement, image PNG, CSV |

---

Programme publié automatiquement à partir des sources TalkTrueFPV (dépôt privé). Ce dépôt ne contient que le
programme à télécharger. © TalkTrueFPV.
