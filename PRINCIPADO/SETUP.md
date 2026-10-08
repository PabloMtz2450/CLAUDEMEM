# ?? INSTRUCCIONES - Equipo PRINCIPADO

## Estado Actual
? Rama PRINCIPADO creada en repositorio central  
? Estructura de carpetas lista  
? Archivo de configuración preparado  

## PARA EL OTRO EQUIPO (con dominio)

### Paso 1: Clonar el repositorio
\\\powershell
cd C:\Users\pablo
git clone https://github.com/PabloMtz2450/CLAUDEMEM.git
cd CLAUDEMEM
\\\

### Paso 2: Cambiar a rama PRINCIPADO
\\\powershell
git checkout principado
\\\

### Paso 3: Configurar el usuario Git
\\\powershell
git config user.name "Pablo Martinez"
git config user.email "juan.martinez@principado.com.mx"
\\\

### Paso 4: Establecer variable de entorno
\\\powershell
[Environment]::SetEnvironmentVariable('CLAUDE_EQUIPO', 'principado', 'User')
\\\

### Paso 5: Copiar script de auto-sync
Copiar desde Aracno:
\\\
C:\Users\Pablo\AppData\Local\Claude\claude-auto-sync.ps1
\\\

O crear uno nuevo con:
\\\powershell
C:\Users\Pablo\AppData\Local\Claude\claude-auto-sync.ps1 -Equipo principado
\\\

### Paso 6: Primera sincronización
\\\powershell
C:\Users\Pablo\AppData\Local\Claude\claude-auto-sync.ps1 -Equipo principado
\\\

### Paso 7: Verificar
\\\powershell
git status
git log --oneline -1
\\\

## ? Listo

A partir de ahora:
- Cada sesión sincronizará automáticamente
- Los chats y memorias se guardarán en PRINCIPADO/
- Puedes ver el historial de Aracno con: \git checkout aracno\
- Todo está sincronizado en: https://github.com/PabloMtz2450/CLAUDEMEM

## ?? Repositorio
https://github.com/PabloMtz2450/CLAUDEMEM

Rama PRINCIPADO: https://github.com/PabloMtz2450/CLAUDEMEM/tree/principado
