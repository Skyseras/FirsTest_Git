GitLab:

 1. Developed by: GitLab was developed by Dmitriy Zaporozhets and Valery Sizov.
 2. Open source: GitLab is open-source for community edition.
 3. Public Repository: It allows users to make public repositories.
 4. Private Repository: GitLab also provides a free private repository.
 5. Navigation: GitLab provides the feature of navigation into the repository.
 6. Project Analysis: GitLab provides users to see project development charts.
 7. Advantages: - GitLab is freely available and open is source for community edition
		- It is a cloud-native application and is highly secure.
 8. Disadvantages: - GitLab is available with many bugs and it makes user experience sloppy.
		- It is difficult to manage code reviews for the first timers.

GitHub:

 1. Developed by: GitHub was developed by Chris Wanstrath, Tom Preston-Werner, P. J. Hyett, and Scott Chacon.
 2. Open source: GitHub is not open source.
 3. Public Repository: It allows users to have unlimited free repository.
 4. Private Repository: GitHub allows users to have a free private repository but with a maximum of three collaborators.
 5. Navigation: GitHub allows users to navigate usability.
 6. Project Analysis: GitHub doesn’t have this feature yet but they can check the commit history.
 7. Advantages: - It helps us create an organized document for the project.
		- It is used for sharing the work in front of the public.
 8. Disadvantages: - There is a limited private repository.
		- It supports only Git version control.


Commandes GIT:

Git config
On l’utilise pour configurer les préférences de l’utilisateur : son mail, l’algorithme utilisé pour diff, le nom d’utilisateur et le format de fichier etc.
git config --global user.email sam@google.com

Git init
Cette commande est utilisée pour créer un nouveau dépôt GIT.

Git add
La commande git add peut être utilisée pour ajouter des fichiers à l’index. Par exemple, git add temp.txt

Clone git
La commande git clone est utilisée pour la vérification des dépôts. Si le dépôt se trouve sur un serveur distant, utilisez:
git clone alex@93.188.160.58:/chemin/vers/dépôt
Inversement, si une copie de travail d’un dépôt local doit être créée, utilisez:
git clone /chemin/vers/dépôt

Git commit
La commande git commit permet de valider les modifications apportées au HEAD. Exemple: git commit –m “Description du commit”

Git status
La commande git status affiche la liste des fichiers modifiés ainsi que les fichiers qui doivent encore être ajoutés ou validés.

Git push
Un simple push envoie les modifications locales apportées à la branche principale associée : git push origin main.

Git checkout
La commande git checkout peut être utilisée pour créer des branches ou pour basculer entre elles. Par exemple nous allons créer une branche:
command git checkout -b <nom-branche>
Pour passer simplement d’une branche à une autre, utilisez:
git checkout <nom-branche>

Git remote
Cette commande remote permet à un utilisateur de se connecter à un dépôt distant. git remote –v

Git branch
La commande git branch peut être utilisée pour répertorier, créer ou supprimer des branches. Pour répertorier toutes les branches présentes dans le dépôt, utilisez:
git branch
Pour supprimer une branche:
git branch –d <nom-branche>

Git pull
Pour fusionner toutes les modifications présentes sur le dépôt distant dans le répertoire de travail local.

Git merge
La commande git merge est utilisée pour fusionner une branche dans la branche active. Usage:
git merge <nom-branche>

Git diff
La commande git diff permet de lister les conflits. Pour visualiser les conflits d’un fichier, utilisez
git diff --base <nom-fichier>
La commande suivante est utilisée pour afficher les conflits entre les branches à fusionner avant de les fusionner:
git diff <branche-source> <branche-cible>
Pour simplement énumérer tous les conflits actuels, utilisez:
git diff

Git tag
Le marquage est utilisé pour marquer des commits spécifiques avec des poignées simples. Un exemple peut être:
git tag 1.1.0 <insert-commitID-here>

Git log
L’ exécution de cette commande génère le log d’une branche. Un exemple de sortie :
commit 15f4b6c44b3c8344caasdac9e4be13246e21sadw 
Author: Alex Hunter <alexh@gmail.com> 
Date: Mon Oct 1 12:56:29 2016 -0600

Git reset
Pour réinitialiser l’index et le répertoire de travail à l’état du dernier commit, la commande git reset est utilisée :
git reset --hard HEAD

Git rm
Git rm peut être utilisé pour supprimer des fichiers de l’index et du répertoire de travail. Usage:
git rm nomfichier.txt