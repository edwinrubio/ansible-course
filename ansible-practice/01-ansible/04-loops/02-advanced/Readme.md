# Aqui los que se va a hacer es crear usuario desde una lista
ansible-playbook -i ../../hosts.txt agregar-usuarios.yaml

# Verificamos que los cambios se hallan generado
ansible all -i ../../hosts.txt -m command -a "tail -3 /etc/passwd"