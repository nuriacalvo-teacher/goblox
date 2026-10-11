# GOBLOX

Un juego al estilo Roblox para practicar inglés con situaciones reales (*scenario-based learning*). Cada alumno entra con su cuenta de iesgoya.es, juega misiones, gana GOYUX y construye su propio país angloparlante.

- **Misiones:** *Healthy Bites Diner* (restaurante) y *Back to School Rush* (tiendas). Hay tres dificultades y las sorpresas cambian en cada partida.
- **My Nation:** cada alumno funda su país en una isla 3D. Para construir cada edificio tiene que aprobar un test de inglés.
- **Panel del profesor:** clases con código, GOYUX por buen comportamiento, historial de partidas, invitados y profesores del departamento.

## Archivos

| Archivo | Qué es |
| --- | --- |
| `index.html` | El juego completo. En Apps Script se pega en un archivo HTML llamado `index`. |
| `apps-script/Code.gs` | El servidor. Guarda todo en la hoja de cálculo de Google. |
| `apps-script/LEEME.md` | Instrucciones paso a paso para instalarlo y usarlo en clase. |

## Instalación

Sigue [`apps-script/LEEME.md`](apps-script/LEEME.md). En resumen:

1. Crea una hoja de cálculo de Google y abre **Extensiones → Apps Script**.
2. Pega `apps-script/Code.gs` en `Código.gs` y cambia `ADMINS` por tu correo.
3. Crea un archivo HTML llamado `index` y pega `index.html`.
4. Ve a **Implementar → Nueva implementación → Aplicación web**, con *Ejecutar como: Yo* y *Acceso: cualquier usuario de IES Goya*.
5. La URL que termina en **`/exec`** es el enlace del juego. Compártela con los alumnos.

## Enlaces

- **Enlace para jugar (alumnos):** *pega aquí la URL `/exec` de la implementación*
- **Enlace para invitados (opcional):** *pega aquí la URL `/exec` de la segunda implementación*

La URL del editor de Apps Script (`script.google.com/.../edit`) es solo para ti y no hay que ponerla en ningún archivo.
