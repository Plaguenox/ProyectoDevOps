# Proyecto Ansible: Servidor DevOps InnovaSys

Este proyecto automatiza la configuración de un servidor Ubuntu 24.04 para la startup InnovaSys, cumpliendo dos funciones clave:

- 🌐 Portal de bienvenida interno (Apache)
- 📂 Repositorio de archivos compartido (Samba)

## Requisitos

- Nodo de control: Linux Lite con Ansible
- Nodo gestionado: Ubuntu Server 24.04
- Acceso SSH con privilegios sudo

## Estructura

- `roles/apache`: instala Apache y genera una página HTML personalizada
- `roles/samba`: configura Samba, crea usuarios, grupos y recursos compartidos

## Ejecución

```bash
ansible-playbook playbooks/servidor.yml -i inventario/hosts
