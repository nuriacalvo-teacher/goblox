# GOYALAND

Un juego al estilo Roblox para practicar inglés con situaciones reales (*scenario-based learning*). Cada alumno entra con su cuenta de iesgoya.es, juega misiones, gana GOYUX y construye su propio país angloparlante.

- **Misiones:** *Healthy Bites Diner* (restaurante, EE. UU.), *Back to School Rush* (tiendas), *A&E: Emergency!* (urgencias en Manchester), *Hotel Trouble* (hotel en Edimburgo), *Lost in London* (metro de Londres), *Airport Check-in* (aeropuerto de Dublín), *Movie Night* (cine en Toronto), *New School in Dublin* (primer día de instituto) *Join the Gym* (gimnasio en Sídney), *My Host Family* (Cork), *Stay Safe: Ask for Help* (Mánchester), *Report a Theft* (Edimburgo), *Lost Passport* (Londres), *Noisy Neighbours* (Toronto), *At the Bank* (Sídney), *At the Print Shop* (imprenta en Wellington, Nueva Zelanda), *First Date* (primera cita en Brighton), *At the Supermarket* (supermercado en Cardiff, Gales), *At the Florist* (floristería en Vancouver), *Garden Centre* (centro de jardinería en Bristol), *At the Pharmacy* (farmacia en Boston), *Birthday Party Plans* (Liverpool), *Phone Shop Problem* (Los Ángeles) y *Guided City Tour* (York). En estas misiones, y en *At the Print Shop*, *First Date* y *At the Supermarket*, cada nivel es una historia distinta (otro motivo, otros problemas y otro registro). Hay tres dificultades (A2, B1 y B2–C1) y las sorpresas cambian en cada partida. En las misiones nuevas, el registro cuenta: ser demasiado formal con la familia o demasiado brusco con un policía resta modales. Los tratados entre países incluyen una misión especial larga (comercio, cultura o paz) y dan 1000 GOYUX. En la portada hay además 49 situaciones marcadas como *in development* (deporte, espectáculos, arte, compras, seguridad personal, vida cotidiana…).
- **Cromos:** al terminar una misión con 65 puntos o más, el alumno gana su cromo de ese nivel (bronce = Easy, plata = Normal, oro = Hard). Ganar el cromo da 40, 60 u 80 GOYUX según el nivel (180 entre los tres: una parcela y un edificio) (una sola vez). Repetir ese nivel sirve para practicar, pero ya no da GOYUX.
- **Desbloqueo:** al principio solo está abierta la primera misión en Easy. Cada cromo abre el nivel siguiente de esa misión y el mismo nivel de la misión siguiente.
- **My Nation:** cada alumno funda su país en una isla 3D. Para construir cada edificio tiene que aprobar un test de inglés.
- **Panel del profesor:** clases con código, GOYUX por buen comportamiento, historial de partidas, invitados y profesores del departamento.

## Archivos

| Archivo | Qué es |
| --- | --- |
| `index.html` | La portada de **https://nuriacalvo-teacher.github.io/goyaland/**. Lleva a los alumnos al juego de Apps Script. |
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

Da a los alumnos **https://nuriacalvo-teacher.github.io/goyaland/**. La portada tiene dos botones: **Students** lleva al juego de Apps Script (`/exec`), donde entran con su cuenta de iesgoya.es y todo se guarda en tu hoja; **Guests** es para quien entra con un código de invitado.

- El enlace `/exec` está escrito en `index.html` (línea `GAME_URL`). Si algún día creas una implementación nueva con otra URL, cámbiala ahí.
- **Invitados** (sin cuenta de iesgoya.es): el mismo enlace, botón *Guests: play with an invite code*. Lleva a la segunda implementación (`GUEST_URL` en `index.html`).
- La portada incluye una **demo sin conexión** (`apps-script/index.html`) para probar el juego sin cuenta. En la demo no se guarda nada.

La URL del editor de Apps Script (`script.google.com/.../edit`) es solo para ti.
