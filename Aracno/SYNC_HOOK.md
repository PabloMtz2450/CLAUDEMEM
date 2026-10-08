# Hook de Sincronización SessionStart

Este hook sincroniza automáticamente la memoria de la rama PRINCIPADO
al inicio de cada sesión cuando trabajas en Aracno.

## Configuración

El hook está en: ~/.claude/settings.json

Script: C:\Users\Pablo\AppData\Local\Claude\sync-principado-memory.ps1

## Cómo funciona

1. Al iniciar sesión en Aracno, el hook se ejecuta automáticamente
2. Trae la memoria de PRINCIPADO usando git show
3. La copia a Aracno/memory/PRINCIPADO_ref/
4. No cambia de rama, solo referencia

## Acceso

Los archivos de PRINCIPADO están siempre disponibles en:
C:\Users\pablo\CLAUDEMEM\Aracno\memory\PRINCIPADO_ref\

Para ver la rama PRINCIPADO original:
git checkout principado
