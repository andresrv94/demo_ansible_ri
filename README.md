# Demo Ansible/Vagrant DevOps

Pasos a seguir para reproducir la demo:

- Instalar Ansible, Vagrant y Virtualbox
- Clonar este repositorio
- Verificar si tenemos clave RSA generada mediante el comando:

        ls -l ~/.ssh
- Si tenemos los archivos id_rsa y id_rsa.pub continuar, sino ejecutar el siguiente comando

        ssh-keygen


- Entrar a la carpeta donde se ubica el Vagrantfile y ejecutar el siguiente comando para inicializar las máquinas virtuales:

        vagrant up

- Finalizado el proceso ejecutar el playbook de Ansible

        ansible-playbook playbook.yml -u vagrant -i inventory

- Para apagar las VMs ejecutar el siguiente comando

        vagrant halt

- Para destruirlas ejecutar el siguiente

        vagrant destroy

