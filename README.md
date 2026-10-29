# Cinco servidores Ubuntu automatizados con Ansible

## Ejecución

1. Inicie los servidores: `docker compose up -d --build`.
2. Instale Ansible y `sshpass` en WSL: `sudo apt update && sudo apt install -y ansible sshpass`.
3. Compruebe acceso: `ansible servidores -m ping`.
4. Ejecute: `ansible-playbook playbook.yml`.
5. Verifique: `ansible servidores -a 'cat /home/itla/app/hola.txt'`.
6. Detenga el laboratorio: `docker compose down`.

La contraseña `ansible` es deliberadamente didáctica y solo se usa en contenedores locales descartables.
