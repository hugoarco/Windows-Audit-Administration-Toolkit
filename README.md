<h1 align ="center">Windows Audit & Administration Toolkit</h1> 

Toolkit completo para la preparación, auditoría y administración de sistemas Windows en entornos educativos y empresariales.

## Descripción

Este proyecto recoge todo el proceso de preparación y auditoría de un sistema Windows, desde la creación de usuarios y grupos hasta la generación de informes automatizados con scripts de PowerShell. Diseñado para entornos educativos (SMR/ASIR) pero funcional en entornos profesionales.

## Scripts incluidos

1. Script-Crear-Estructura.ps1 - Crea la estructura C:\SMR-AULA con todas las subcarpetas
2. Script-Auditoria-Basica.ps1 - Recoge información del sistema (systeminfo, ipconfig, tasklist, servicios)
3. Script-Auditoria-Completa.ps1 - Auditoría completa: usuarios, grupos, permisos, software instalado

## Áreas cubiertas

- Usuarios y grupos locales (net user, net localgroup)
- Estructura de carpetas y permisos NTFS (icacls)
- Instalación de software con Winget (7-Zip, VLC, Git, VS Code)
- Diagnóstico de red (ping, ipconfig, tracert, nslookup)
- Gestión de procesos (tasklist, taskkill)
- Copias de seguridad (manual, ZIP, robocopy, script)
- Directivas de seguridad local (secpol.msc)
- Scripts automatizados de auditoría

## Requisitos

- Windows 10/11 (Pro recomendado para directivas)
- PowerShell 5.1 o superior
- Ejecutar como Administrador
- Winget (incluido en Windows 10/11 modernos)

## Cómo usar

1. Abre PowerShell como Administrador
2. Ejecuta: Set-ExecutionPolicy RemoteSigned -Scope CurrentUser -Force
3. Ejecuta los scripts en orden:
   .\Script-Crear-Estructura.ps1
   .\Script-Auditoria-Basica.ps1
   .\Script-Auditoria-Completa.ps1
4. Revisa los informes generados en C:\SMR-AULA\Auditoria\

## Autor

Hugo Arco
GitHub: https://github.com/hugoarco
Email: hugoultecno@gmail.com

## Licencia

MIT License

## Estado

✅ Completado – Totalmente funcional y documentado
## Diagrama de Flujo 
<img width="3208" height="2660" alt="diagram (1)" src="https://github.com/user-attachments/assets/313fc630-fe04-46b3-a97d-68c39d8ad649" />
