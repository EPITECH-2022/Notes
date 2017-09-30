# Comment installer Discord?

## Technique 1

Vous voulez télécharger Discord sur votre machine Fedora? Suivez ce petit tuto:

Premièrement, allez sur la page suivante: https://discordapp.com/download
Vous l'avez deviné, nous allons le télécharger. Choisissez le format `.tar.gz`

Une fois ceci fait, décompressez l'archive où bon vous semble. Fait en sorte de rendre le script nommé `Discord` executable
N'essayez-pas de le lancer, vous n'y arriverez pas. Et ce pour une raison simple: Il manque une dépendance.

Pas de panique! Elle est facile à récupérer. Lancez la commande suivante: `sudo dnf install libcxx`
Une fois l'installation faite, bien joué! Vous pouvez enfin accèder à Discord sur votre machine!

## Technique 2

Vous faites `git clone https://github.com/RPM-Outpost/discord ~/discord && cd ~/discord && ./create-package.sh canary` (faites "yes yes yes yes...") et c'est tout

Technique proposé par Tina

# Comment installer i3?

Tina à proposé sa config i3 ainsi qu'un tuto sur [son GitHub](https://github.com/skielred/Dotfiles)
