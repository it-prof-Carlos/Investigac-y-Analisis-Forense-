








































































  Volatility: Análisis de volcados de memoria
    Análisis y extracción de artefactos forenses Windows
    
    
    Velociraptor: Recolección, idnetificación  y hunting sobre investigación y analisis forense digital y respuesta a incidentes windows
    
    
    LogonTracer: Trazabilidad de inicios de sesión en Active Directory
    

    Skadi: Análisis de artefactos e imágenes forenses
    GRR - Google Rapid Response
    

    Live Forensicator - Recolección automatizada de información y artefactos en Windows, Linux y MacOS
    EnCase Forensic (ondata)
    
    
    SANS DFIR - Posters \& Cheat Sheets

 Ejecución de otras técnicas  CMD - PowerShell
    
 Bloquear conexiones USB: Rubber Ducky y Cactus WHID

 Claves de registro de Windows donde se almacenan las contraseñas
 WDigest Authentication: Habilitado / Deshabilitado

Identificacion sobre sistema en implementación en máquina física o virtual  (Azure, AWS, GCP)
    
Identificacion sobre sistema en implementación en  máquina física o virtual, tipo de hipervisor o CSP  (Azure, AWS, GCP)


Linux

*debugfs* para eludir alertas al ejecutar comandos o acceder a ficheros con auditoria
```bash
df -h
sudo debugfs /dev/sda1
debugfs: ls
debugfs: cat /etc/passwd
... modo interactivo ...

```bash
$ sudo bash malware.sh
$ history
    1  clear
    2  sudo bash malware.sh
    3  history
```

Auditoría en el uso  de los siguientes comandos  Linux

Los siguientes comandos privilegiados deberían auditarse:
|   |   |   |   |   |   |

| agetty | cvsbug | fdisk | ipcs | mkswap | quotacheck |
| arp | debugfs | fsck | lpc |mountd | quotaoff |
| badblocks | dmesg | ftpd | lpd | nfsd | quotaon |
| Cfdisk | dumpe2fs | inetd | makedev | nslookup | renice | 
| Chroot | e2fsck | init | mke2fs | overchan | repquota |
| Crond | edquota | nndstart | mkfs | plipconfig | rpcinfo |
| ctrlaltdel | fdformat | ipcrm | mklost+found | portmap |


Redes

WAF Bypass (SSRF): usar acortamiento IP local

| Bloqueo            | Bypass           |
|--------------------|------------------|
| http://10.0.0.1    | http://1.1       |
| http://127.0.0.1   | http://127.1     |
| http://192.168.0.5 | http://192.168.5 |

Dirección IPv6 asignada a IPv4 utilizada para ofuscación

Una dirección IPv6 se puede asignar a una dirección IPv4. Por lo tanto, si un actor malicioso intenta reconocer un servidor para conectarse a una dirección IPv4 y es bloqueado por la solución de seguridad. Probar esta técnica para ofuscar la comunicación y evitar posibles detecciones.

```
ping ::ffff:8.8.8.8
Haciendo ping a 8.8.8.8 con 32 bytes de datos:
Respuesta desde 8.8.8.8: bytes=32 tiempo=13ms TTL=117
```

La parte de IPv4 también se puede convertir a hexadecimal.
``` 
ping ::ffff:0808:0808
Haciendo ping a 8.8.8.8 con 32 bytes de datos:
Respuesta desde 8.8.8.8: bytes=32 tiempo=13ms TTL=117
```

Forensia (Anti-Forensic)