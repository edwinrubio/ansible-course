# Los handlers son detenccion de eventos si determinada cosa se notifica a un handler
ansible-playbook -i ../../hosts.txt handler-exmaple.yaml
# Para verificar que todo halla salido bien corremos el siguiente comando
ansible vm1 -i ../../hosts.txt -m command -a "id edwin"
