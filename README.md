# vim-ide

Toute la configuration et les plugins pour faire un bon ide avec vim

## Installation

Faire un backup de l'ancienne configuration :
<code>
mv ~/.vimrc ~/.vimrc.old
mv ~/.vim ~/.vim.old
</code>

Cloner le repository puis créer un lien symbolique :

<code>
ln -s <path-to-repository> ~/.vim
ln -s <path-to-repository>/vimrc ~/.vimrc
</code>

## Utilisation

On se place dans le répertoire de travail.

Pour avoir la reconnaissance des methodes, propriétés etc... on utilise ctags
On met le fichier généré dans le répertoire git comme ça il ne nous gène pas

Pou pouvoir utiliser ctags, il faut installer le paquet exuberant-ctags.

Puis :
<code>
ctags -R -f ./.git/tags .
</code>

Et on lance gvim.

Ctrl+n => Pour ouvrir le navigateur de fichier 
        navigation au clavier ou à la souris  dans les repertoires
        
Ctrl+b => Pour ouvrir "l'outline"

,+t => recherche de fichier intélligente grace à [command-t](https://wincent.com/products/command-t) recherche de fichier style sublime text

Ctrl+tab / Ctrl+shift+tab => tab suivante / précedente (ça boucle sur les tabs)
