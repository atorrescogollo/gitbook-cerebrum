# Módulos de Ansible

## Depuración de módulos con VSCode

> Fuente: [https://docs.ansible.com/ansible/latest/dev\_guide/debugging.html](https://docs.ansible.com/ansible/latest/dev_guide/debugging.html)

1. Ejecutar el playbook con `ANSIBLE_KEEP_REMOTE_FILES`

```bash
export ANSIBLE_KEEP_REMOTE_FILES=1
ansible-playbook playbook.yml -vvvv
```

Buscamos un fichero parecido a esto:  
`/home/../.ansible/tmp/ansible-tmp-<timestamp>/AnsiballZ_<module>.py`

2. Descomprimir el `AnsiballZ` y abrir en VSCode

```bash
cd /home/atorres/.ansible/tmp/ansible-tmp-<timestamp>/
./AnsiballZ_<module>.py explode
code . # Abrir VSCode
```

3. Ejecutar la depuración

* Lo primero es **poner el breakpoint donde queramos**.
* Luego, ejecutamos el fichero con la siguiente configuración de VSCode:

  ```javascript
  {
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Python: Current File",
            "type": "python",
            "request": "launch",
            "program": "AnsiballZ_<module>.py",
            "console": "integratedTerminal",
            "args": [
                "execute"
            ]
        }
    ]
  }
  ```



