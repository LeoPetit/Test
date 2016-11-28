COnfiguration : git config [type] def [valeur]
type : --system : pour tous les utilisateurs du systeme
       --global : pour tous les depots de l'utilisateur
       --local : pour un depot donné
       
$ git config --global def user.name "Prénom nan"
$ git config --global user.email "user@exemple.com"
$ git config --global color.ui auto


Différentes maniere pour désigner un commit :
-> identifiant evenuellement abrégé
ex : $git show 37efa8
     $git diff 3754654 6498484
    
nom de branche : dernier commit de la branche donnée
ex : $git show experimental

HEAD : dernier commit de la branche courante
commit^ : commit précédent celui donné
ex : $git show HEAD
     $git show HEAD^
     $git show HEAD^^

commit ~ numérosCommit : équivalent à commit ^^...^^(n chapeau)

On peu aussi donnée un nom étiquetter d'un commit : 
$git tag v2.5 37e6546
-donne le nom v2.5 au commit 37e6546
$git show v2.5

crée une branche qu'on appele stable a partire des 2.5

Autres commandes utiles :
Rechercher dans un fichier :
       $git grep

Void qui a modifier le fichier :
$git blame fichier

Retrouver le commit ayant introduit un probleme :
$git bisect
usage simple :
$git bisect start
$git bisect bad
$git bisect goot v2.5



















