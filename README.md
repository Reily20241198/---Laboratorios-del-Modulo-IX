# ---Laboratorios-del-Modulo-IX
Practica 5: Playbooks (1Pts)
Práctica Ansible - Comandos y Significados

1. ansible linux -m ping
   - Significado: Verifica la conectividad con los hosts del grupo "linux" usando el módulo ping de Ansible.

2. ssh-copy-id -i ~/.ssh/id_rsa_ansible.pub ansible@192.168.0.116
   - Significado: Copia la clave pública SSH al servidor remoto para permitir acceso sin contraseña.

3. ansible linux -m reboot
   - Significado: Reinicia las máquinas del grupo "linux" usando el módulo reboot.

4. ansible win -m win_ping
   - Significado: Verifica la conectividad con hosts Windows usando el módulo win_ping.

5. Set-Item -Path WSMan:\localhost\Service\Auth\Basic -Value $true (en PowerShell Windows)
   - Significado: Habilita la autenticación básica para WinRM en Windows.

6. Set-Item -Path WSMan:\localhost\Service\AllowUnencrypted -Value $true (en PowerShell Windows)
   - Significado: Permite la comunicación no cifrada en WinRM para facilitar conexiones.

7. net localgroup administrators ansible /add (en PowerShell Windows)
   - Significado: Agrega el usuario "ansible" al grupo de administradores locales en Windows.

8. ansible-playbook install_notepadpp_win.yml
   - Significado: Ejecuta un playbook de Ansible para instalar Notepad++ en la máquina Windows.

9. ansible-playbook install_nginx_linux.yml
   - Significado: Ejecuta un playbook de Ansible para instalar y arrancar el servicio NGINX en la máquina Linux.

10. systemctl status nginx.service (en Linux)
    - Significado: Muestra el estado actual del servicio NGINX.

11. sudo ss -tulpn | grep :8080 (en Linux)
    - Significado: Muestra qué proceso está escuchando en el puerto 8080.

12. ansible win -m win_shell -a "Copy-Item -Path '...' -Destination '...'"
    - Significado: Ejecuta un comando PowerShell remoto en Windows para copiar un archivo.

13. ansible linux -m shell -a "systemctl status nginx"
    - Significado: Ejecuta un comando shell remoto en Linux para consultar el estado de NGINX.

14. ansible linux -m shell -a "curl http://localhost"
    - Significado: Ejecuta una consulta HTTP local en Linux para verificar que el servidor web esté respondiendo.

15. winrm quickconfig -q (en Windows PowerShell)
    - Significado: Configura WinRM para permitir la administración remota.

16. winrm set winrm/config/service/auth @{Basic="true"} (en Windows PowerShell)
    - Significado: Configura WinRM para permitir autenticación básica.

17. winrm set winrm/config/service @{AllowUnencrypted="true"} (en Windows PowerShell)
    - Significado: Permite que WinRM use comunicaciones sin cifrar.

18. net user ansible "P@ssw0rd123" /add (en Windows PowerShell)
    - Significado: Crea un usuario llamado "ansible" con la contraseña especificada.

19. net localgroup "Remote Management Users" ansible /add (en Windows PowerShell)
    - Significado: Agrega el usuario "ansible" al grupo de usuarios permitidos para administración remota.
