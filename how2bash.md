# Linux in a nutshell

## On passe son temps à me dire de taper des commandes dans un terminal. C'est quoi?

Un terminal, c'est le meilleur moyen de communiquer avec la machine.
C'est une boite, avec que du texte. Tu peux taper des trucs, et des fois ça t'en montre en réponse.

## Mais ça m'a l'air compliqué tout ça!

Ouai mais non, t'en fait pas, on s'y habitue vite.

# Les bases du filesystem

Premièrement, il faut savoir se déplacer.

Les premières commandes seront donc sur le déplacement dans le filesystem.

## Comment ça marche?

Premièrement, il est important de comprendre comment un disque dur est agancé sur Linux.
La racine du système, c'est `/`. Tout commence de la.
Ensuite, il y a un dossier important, *votre* dossier `home`. Celui-ci est dans /home/VotreUtilisateur. Dedans, vous y avez à peu près tout les droits
Pour faire simple, vous pouvez utiliser `~` pour signifier votre dossier home. (Par exemple, si vous êtes l'utilisateur `cola`, et bien `/home/cola/Desktop` est exactement la même chose que `~/Desktop`)

L'exemple du home va me permetre de faire la différence entre chemin absolu et chemin relatif.
Les fichiers ont un chemin absolu sur le disque. C'est leur emplacement exact. Leur chemin commence toujours par un / (signifiant le début du disque)
C'est comme si vous avez un fichier `C:\Machin\Truc\Bidule.txt` sur Windows.
Sur Linux, vous avez aussi les chemins relatifs. Soit relatif à votre home (~), ou relatif à votre emplacement actuel dans un terminal.
Imaginez, dans votre terminal, vous êtes dans le dossier `Machin` de l'exemple précédent. Pour signifier le dossier `Truc`, pas besoin du chemin absolu. Si vous faite `./Truc`, il va comprendre.
Vous l'avez compris, faire `./` signifie `Le dossier dans lequel je me trouve actuellement`

Imaginez maintenant que nous sommes dans `Truc`, et qu'en réalité, il y ai un dossier `/Machin/Chouette`. Au lieu de redonner son chemin absolu, vous pouvez aussi en faire mention avec `../Chouette`. Oui, l'option `../` signifie le dossier parent

[Voici une représentation imagée du filesystem](https://i.imgur.com/bsWYdmJ.jpg) si ça vous intéresse. Ne l'apprenez pas par coeur pour le moment. Retenez juste que le home est votre maison.

## Où que je suis? Comment je vais la-bas?

Par défaut, dans votre terminal, vous êtes dans `~`.

Pour changer de dossier, faites `cd DossierDeDestination`. Evidemment, cela supporte les chemins absolu et relatifs.
Si vous êtes perdu, utilisez `pwd` pour connaitre votre position.

# Les autres commandes

Premièrement, avant de poser la moindre question à qui que ce soit, lisez ce readme, et surtout
Utilisez `man`. `man`, c'est le petit nom de `Manuel`. Une question sur une commande? `man commande`.
Vous trouvez toujours pas? Google it.
Toujours pas? La vous pouvez demander.

## Je veux installer un paquet, je fais comment?

Pour installer un paquet, vous avez besoin de `YUM`, qui lui-même demande les permissions admin (Cf. linux101.md)
La syntaxe est `sudo dnf install paquet` pour un paquet sur un repo. Si jamais vous avez un fichier RPM, c'est `sudo dnf install LeCheminDeVotre.rpm`.

Pour retirer un paquet, `sudo dnf remove NomDuPaquet`.
