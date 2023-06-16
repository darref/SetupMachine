# Installation des composants WSL , git , extension WSL pour VS code , et preparation d'un projet github avec clé SSH.

## installer wsl:
- cherchez wsl2 dans google et recopiez la commande wsl --install
- la coller dans un invité de commande ouvert en mode administrateur
- executer la commande
- si vous obtenez l'erreur ``WslRegisterDistribution failed with error: 0x80004002
Error: 0x80004002 Cette interface n?est pas prise en charge``
executez la commande :
``
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
``
cette commande va redemarrer votre pc.
- une fois le pc redemarré executez ubuntu et vous aurez un message qui vous demande d autoriser les machines virtuelles dans votre bios
- une fois cela fait , executez ubuntu , il vous sera demandé de chosiir un login et un mot de passe que vous devrez entrer 2 fois.


## installer git:

- chercher git scm dans google 
- aller dans downloads
- Cliquer sur "Latest souce release" (download for windows)
- choisir la version 32 ou 64 bit en fonction de votre os
- installer en cliquant sur suivant , suivant ...

## initialiser github:

- aller sur github.com
- creer un compte ou connectez vous a votre compte
- créer un nouveau projet privé ( cliquer sur New )
- dans le projet , aller dans settings
- maintenant allez dans cmd ( bouton windows et taper cmd pui entrer)
- dans votre machine virtuelle ubuntu , placez vous (a l aide de la commande cd) dans le dossier ou vous voulez creer la clé ssh
- dans la console , tapez ssh-keygen puis entrer
- on vous demander de choisir un chemin ou exporter les clés publiques et pivées , puis appuyez sur entrer
- choisir un mot de passe et le rentrer deux fois ( mot de passe invisible lors del a saisie , c'est normal)
- ouvrez la  cle publique et copier son contenu
- le coller sur le site de github dans la section settings > deploy keys > add deploy key et validez en cliquant sur le bouton add.
  
  ![df](./images/Capture%20d%E2%80%99%C3%A9cran%202023-06-16%20103641.png)