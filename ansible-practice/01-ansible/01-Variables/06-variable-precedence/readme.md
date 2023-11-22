# Ahora ejecutamos este comando para ver como podemos sobreescribir una variable desde comandos
ansible-playbook -i ../../hosts.txt variable-precendence.yml -e "fav_distro=CentOS"