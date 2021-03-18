# TP-Ansible

Dans ce dépôt, vous pourrez retrouver les fichiers utilisés pour le TP Ansible.

## Info 

Pour clôner ce dépôt (le télécharger sur votre machine), vous devrez installer GIT.\
`sudo apt install git`

Ensuite, vous devrez cloner mon dépôt avec git, pour cela, entrez la commande suivante:\
`git clone git@github.com:AlbanVidalenche/TP-Ansible.git`

Cette commande va créer un dossier contenant le code utilisé dans le tp. Vous pourrez utiliser ce dossier pour faire des tests si vous obtenez des erreurs.

 :warning: Le code sera régulièrement modifié au fur et à mesure du cours, pour être sûr que vous utlisez bien la dernière version du code, pensez à effectuer la commande suivante avant de faire vos tests. Cette commande doit être réalisée dans le dossier TP-Ansible.
`git pull`

Si des modifications ont été effectuées, le dossier sera mis à jour.


# Problèmes de forwarding de clés SSH 

Si la commande `ssh-add` ne fonctionne pas sur windows et renvoie l'erreur suivante : `communication with agent failed` \
Comme décrit dans cet article : https://github.com/PowerShell/Win32-OpenSSH/issues/1133 \


Lancez la commande suivante:\
`sc.exe create sshd binPath=C:\Windows\System32\OpenSSH\ssh.exe`

Vous pourrez ensuite relancer la commande `ssh-add` qui devrait maintenant fonctioner.
