# GOBLOX

Un juego al estilo Roblox para practicar inglés con situaciones reales (*scenario-based learning*). Cada alumno entra con su cuenta de iesgoya.es, juega misiones, gana GOYUX y construye su propio país angloparlante.

- **Misiones:** *Healthy Bites Diner* (restaurante) y *Back to School Rush* (tiendas). Hay tres dificultades y las sorpresas cambian en cada partida.
- **My Nation:** cada alumno funda su país en una isla 3D. Para construir cada edificio tiene que aprobar un test de inglés.
- **Panel del profesor:** clases con código, GOYUX por buen comportamiento, historial de partidas, invitados y profesores del departamento.

## Archivos

| Archivo | Qué es |
| --- | --- |
| `index.html` | La portada de **https://nuriacalvo-teacher.github.io/goblox/**. Lleva a los alumnos al juego de Apps Script. |
| `apps-script/index.html` | El juego completo. En Apps Script se pega en un archivo HTML llamado `index`. |
| `apps-script/Code.gs` | El servidor. Guarda todo en la hoja de cálculo de Google. |
| `apps-script/LEEME.md` | Instrucciones paso a paso para instalarlo y usarlo en clase. |

## Instalación

Sigue [`apps-script/LEEME.md`](apps-script/LEEME.md). En resumen:

1. Crea una hoja de cálculo de Google y abre **Extensiones → Apps Script**.
2. Pega `apps-script/Code.gs` en `Código.gs` y cambia `ADMINS` por tu correo.
3. Crea un archivo HTML llamado `index` y pega `apps-script/index.html`.
4. Ve a **Implementar → Nueva implementación → Aplicación web**, con *Ejecutar como: Yo* y *Acceso: cualquier usuario de IES Goya*.
5. La URL que termina en **`/exec`** es el juego de verdad.

## Enlace para los alumnos

Da a los alumnos **https://nuriacalvo-teacher.github.io/goblox/**. Esa portada los lleva automáticamente al juego de Apps Script (`/exec`), donde entran con su cuenta y todo se guarda en tu hoja.

- El enlace `/exec` está escrito en `index.html` (línea `GAME_URL`). Si algún día creas una implementación nueva con otra URL, cámbiala ahí.
- Para invitados, pon la URL `/exec` de la segunda implementación en `GUEST_URL`. Para que la portada no salte sola al juego y se vea el botón de invitado, dales **https://nuriacalvo-teacher.github.io/goblox/?stay**.
- La portada incluye una **demo sin conexión** (`apps-script/index.html`) para probar el juego sin cuenta. En la demo no se guarda nada.

La URL del editor de Apps Script (`script.google.com/.../edit`) es solo para ti.
