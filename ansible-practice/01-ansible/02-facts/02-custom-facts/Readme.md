# Se debe crear el directio /etc/ansible/facts.d dentro de la maquina obejetivo y despues de eso colocar los fact con archivo con extencion fact

# Dentro del playbook se pone el fact 
ansible-playbook -i ../../hosts.txt custom-facts.yaml

# Y se ejecuta con este comando
ansible vm1 -i ../../hosts.txt -m setup -a "filter=ansible_local"