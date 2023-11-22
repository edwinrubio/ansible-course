# Es cuando necesitamos destinar determinadas variables a nodos especificos dentro de la infraestructura
# Entonces creamos archivos de variables con el nombre que le hemos dado al nodo y deben estar dentro de una carpeta llamada host_vars

# Despues de ejecutado el playbook podemos ejecutar este comando para ver si ha funcionado
ansible all -i ../../../hosts.txt -m command -a "cat /etc/motd"