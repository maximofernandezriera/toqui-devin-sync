# toqui-devin-sync

Protocolo privado de relevo entre trabajo local y Devin web. Un solo lado trabaja cada vez. Este repositorio guarda el estado del relevo, no el contenido de los proyectos.

## Límites

- Trabajo local solo cuando el modelo aparece como gratuito. Si exige pago, mejora de plan o consumo de cuota de pago, detenerse y consultar.
- No copiar aquí exámenes, soluciones, datos de alumnado, investigación privada, credenciales ni historiales completos de conversaciones.
- Los archivos de cada proyecto se quedan en su repositorio correspondiente. Aquí basta una referencia al repositorio, rama y commit, sin contenido sensible.
- El protocolo no da permisos nuevos para publicar, enviar mensajes, pagar, acceder a otra cuenta o cambiar un proyecto.
- No hay automatismos, tareas programadas ni sincronización continua instalados. El turno se cambia de forma explícita.

## Archivos

- `ESTADO.md`: turno actual y punto desde el que continuar.
- Este README: procedimiento estable y plantilla para los próximos relevos.

## Tomar el turno

1. Leer la versión remota actual de ESTADO.md. No basarse solo en una copia local antigua.
2. Confirmar que el turno figura libre y que el otro lado ha terminado. Si hay dudas, no empezar a editar el proyecto.
3. Comprobar gratuidad del modo local antes de trabajar.
4. Actualizar ESTADO.md con lado, sesión, objetivo y commit de partida. Guardar ese cambio en GitHub y releer el resultado remoto antes de comenzar.
5. Recuperar los archivos del proyecto desde su propio repositorio y commit. Si hay cambios locales sin guardar o una versión distinta, detener el relevo y conservar ambas versiones.

El turno es una convención de coordinación, no un bloqueo técnico. Si dos sesiones intentan tomarlo a la vez, ninguna debe continuar hasta acordar el propietario. Un cambio de fecha o una sesión desconectada no libera el turno por sí solos.

## Dejar el turno

1. Terminar o detener el trabajo en un punto seguro. No dejar tareas de escritura activas.
2. Guardar los cambios autorizados del proyecto en su repositorio propio, sin mezclar aquí sus archivos. Verificar el commit remoto y el estado de los archivos.
3. Actualizar ESTADO.md: resultado, commit comprobado, cambios aún sin guardar, límites, siguiente paso y lado previsto.
4. Dejar el turno libre solo cuando no quede trabajo activo. Guardar y releer el estado remoto.
5. El lado que recibe confirma que puede leer el estado y los archivos del commit indicado antes de continuar.

## Conflictos y errores

- No usar force push, reset destructivo ni sobrescribir versiones divergentes.
- No dar por sincronizado un archivo por haberlo mencionado en el chat. Comprobar contenido y commit.
- Si el acceso, la gratuidad o el estado remoto no se pueden comprobar, detener solo el paso afectado y comunicar el bloqueo.
- Si una sesión se interrumpe durante una escritura, comprobar primero qué llegó a guardarse antes de repetirla.
- Un archivo histórico puede describir instrucciones antiguas. No ejecutarlas sin una petición vigente.

## Plantilla de estado

```text
Actualizado (fecha, hora y zona):
Turno: libre | local | web | bloqueado
Sesión responsable:
Objetivo autorizado:
Repositorio del proyecto:
Rama del proyecto:
Commit de partida verificado:
Último commit del proyecto comprobado:
Hecho:
Archivos sin guardar o sin subir:
Pendiente:
Siguiente paso:
Lado previsto para recibir:
Bloqueos y decisiones necesarias:
Confirmación de lectura del receptor:
```

No pegar contraseñas, tokens, códigos de verificación ni datos de personas en esta plantilla.

## Qué se ha probado y qué falta

A 18/11/2026 se comprobó un intercambio asistido en ambos sentidos entre una sesión local y Devin web usando GitHub. Eso no demuestra sincronización automática, memoria compartida, fusión de conversaciones ni un `git pull` directo desde el entorno local.

Este repositorio separado se prepara después de esa prueba. Su creación y lectura se verifican por separado; no se presupone que Devin web ya tenga acceso a él. La primera toma real de turno debe comprobar acceso desde ambos lados. No se ha movido ni eliminado la rama histórica de prueba del repositorio anterior.

La disponibilidad gratuita puede cambiar. Si se pierde un entorno local, los archivos y este estado ayudan a reconstruir el trabajo, pero no restauran necesariamente la sesión nativa, sus procesos ni su conversación completa.
