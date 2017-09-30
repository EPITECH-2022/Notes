# Le grand README du Linux EPITECH!

## Pourquoi ce README?

Parce que COLAMAroro, votre admin préferé, en a marre de répondre encore et toujours au mêmes questions. Du coup, bah il fait un README pour vous expliquer les questions courantes.
Vous êtes prêt? C'est partie.

# Linux c'est quoi?

Linux, c'est ce qu'on appel un kernel. En gros, c'est la partie qui s'occupe de communiquer avec l'ordinateur. Seul, il sert à rien. Du coup, les gens on fait ce qu'on appel des **distributions**

## Un distribution? Quel est cette sorcèlerie?

Une distribution, c'est un système d'exploitation "complet", basé sur le kernel Linux. En gros, ils prennent Linux, ils ajoutent les drivers, les logiciels, les utilitaires, les ressources, etc...

Et normalement, vous vous posez la question de la différence entre les distributions. Facile, une distribution ne vient pas avec le même contenu qu'une autre.
Exemple très simple, Fedora vient avec `YUM` comme gestionnaire de paquets (On va revenir sur les paquets), tandis que Debian vient avec `APT`.

De plus, certaines distributions descendent d'autres. Des fois, avec beaucoup de différence (Ubuntu descend de Debian), des fois, vraiment pas beaucoup ([Hannah Montana Linux](http://hannahmontana.sourceforge.net) Descend de Kubuntu, mais inclut juste des thèmes supplémentaires pour KDE)

## Très bien. Et cette histoire de paquet alors?

Un paquet, c'est un logiciel ou une bibliothèque, avec sa documentation. En général, les paquets sont pris en charge par le fameux gestionnaire de paquet (`YUM` pour Fedora).
Le gestionnaire s'occupe de le télécharger, de le lire, de le vérifier, de vérifier ses dépendances (et de les résoudres), et de l'installer.
Les paquets Fedora sont au format .rpm (Pour RedHat Packet Manager, the more you know). La plupart des paquets qui vous intéressent sont sur un "repo" (repository, dépot en français).
Certains paquets, par contre, ne seront pas sur un dépot, mais proposés ailleurs, seuls. Pas de panique, c'est toujours aussi facile de les installer, via la commande `RPM`.

## Et si j'ai pas le paquet, je fais comment? Je pleure?

Oui mais non. Sèche tes larmes. Linux se veut Open Source, et il en va de même pour beaucoup de logiciels. Du coup la plupart des logiciels sont déjà dans un paquet au bon format, sinon, rien ne t'empêche de le compiler toi même.
Regarde les GitHub des projets correspondants. Souvent, ils ont un tuto d'installation/de compilation. Et puis même si il est pas "installé", rien ne t'empêche de prendre un binaire compilé et de le lancer d'où tu veux (comme tu lancerai un fichier .exe depuis ton bureau par exemple)
Et sinon, si tu aime la magie noir, il y a `alien`, qui permet de convertir les paquets d'un format à l'autre, mais c'est un peu buggé. Mais ça existe.
