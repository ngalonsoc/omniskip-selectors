# Política de privacidad de OmniSkip

*English version below.*

Última actualización: 28 de septiembre de 2026

OmniSkip es una extensión para Chrome que salta intros y resúmenes, pasa al siguiente episodio y cierra el aviso «¿Seguís ahí?» en Netflix, Prime Video y HBO Max.

## Resumen

**OmniSkip no recolecta, no vende y no comparte ningún dato personal.** No tiene analítica, no usa cookies propias, no tiene cuentas de usuario y no envía información a ningún servidor del desarrollador.

## Qué se guarda y dónde

Todo queda en tu navegador, usando el almacenamiento de extensiones de Chrome (`chrome.storage`):

| Dato | Dónde | Para qué |
|---|---|---|
| Tus preferencias: extensión activa o en pausa, qué acciones querés en cada plataforma e idioma del popup | `chrome.storage.sync` | Recordar tu configuración |
| Contadores: tiempo ahorrado, cantidad de saltos y fecha de instalación | `chrome.storage.local` | Mostrar el «Tiempo ahorrado» en el popup |
| Copia de los selectores actualizados (ver más abajo) | `chrome.storage.local` | Seguir funcionando si la plataforma cambia sus botones |
| Última pestaña de plataforma que abriste en el popup | Almacenamiento local del popup | Abrir el popup donde lo dejaste |

Si tenés activada la sincronización de Chrome, Google sincroniza tus preferencias (`chrome.storage.sync`) entre tus dispositivos según su propia política de privacidad. El desarrollador de OmniSkip no tiene acceso a esos datos.

Podés poner el contador en cero cuando quieras con el botón «Reiniciar» del popup. Al desinstalar la extensión, Chrome borra todos estos datos.

## Qué hace en las páginas de streaming

OmniSkip solo se ejecuta en Netflix, Prime Video y HBO Max. Ahí busca los botones de «Saltar intro», «Omitir resumen», «Siguiente episodio» y «¿Seguís ahí?» y los presiona según tu configuración. Para no saltar episodios antes de tiempo, lee la duración y el minuto actual del video. **No lee ni guarda qué estás mirando, tu historial, tu cuenta ni ningún otro contenido de la página, y nada de eso sale de tu navegador.**

## Único pedido de red

Una vez por día (y al instalar o actualizar), OmniSkip descarga un archivo JSON público desde:

`https://raw.githubusercontent.com/ngalonsoc/omniskip-selectors/main/selectors.json`

Ese archivo contiene **solo datos**: los nombres de los botones de cada plataforma (selectores CSS), para que la extensión siga funcionando cuando Netflix, Prime Video o HBO Max cambian su página. No contiene código: la extensión lo valida y descarta cualquier cosa que no sea texto.

El pedido se hace sin cookies ni credenciales y no incluye ningún dato tuyo. Como en cualquier conexión a internet, GitHub (el servicio que aloja el archivo) recibe tu dirección IP y datos técnicos del navegador; eso se rige por la [política de privacidad de GitHub](https://docs.github.com/es/site-policy/privacy-policies/github-general-privacy-statement).

## Enlace de donación

El popup tiene un enlace a Ko-fi para donaciones voluntarias. Solo se abre si hacés clic, y a partir de ahí se aplica la política de privacidad de Ko-fi.

## Cambios en esta política

Si la política cambia, se actualiza esta página y la fecha de arriba.

## Contacto

Consultas o dudas: abrí un *issue* en [github.com/ngalonsoc/omniskip-selectors/issues](https://github.com/ngalonsoc/omniskip-selectors/issues).

---

# OmniSkip Privacy Policy

*Versión en español arriba.*

Last updated: September 28, 2026

OmniSkip is a Chrome extension that skips intros and recaps, plays the next episode and dismisses the "Are you still watching?" prompt on Netflix, Prime Video and HBO Max.

## Summary

**OmniSkip does not collect, sell or share any personal data.** It has no analytics, sets no cookies of its own, has no user accounts and sends no information to any server owned by the developer.

## What is stored and where

Everything stays in your browser, in Chrome's extension storage (`chrome.storage`):

| Data | Where | Purpose |
|---|---|---|
| Your preferences: extension on or paused, which actions you want on each platform and the popup language | `chrome.storage.sync` | Remember your settings |
| Counters: time saved, number of skips and install date | `chrome.storage.local` | Show "Time saved" in the popup |
| A copy of the updated selectors (see below) | `chrome.storage.local` | Keep working when a platform changes its buttons |
| The last platform tab you opened in the popup | Popup local storage | Reopen the popup where you left it |

If Chrome sync is turned on, Google syncs your preferences (`chrome.storage.sync`) across your devices under its own privacy policy. The OmniSkip developer has no access to that data.

You can reset the counters at any time with the "Reset" button in the popup. When you uninstall the extension, Chrome deletes all of this data.

## What it does on streaming pages

OmniSkip only runs on Netflix, Prime Video and HBO Max. There it looks for the "Skip intro", "Skip recap", "Next episode" and "Are you still watching?" buttons and presses them according to your settings. To avoid skipping episodes too early, it reads the video's duration and current position. **It does not read or store what you watch, your history, your account or any other page content, and none of it leaves your browser.**

## The only network request

Once a day (and on install or update), OmniSkip downloads a public JSON file from:

`https://raw.githubusercontent.com/ngalonsoc/omniskip-selectors/main/selectors.json`

That file contains **data only**: the names of each platform's buttons (CSS selectors), so the extension keeps working when Netflix, Prime Video or HBO Max change their pages. It contains no code: the extension validates it and rejects anything that is not plain text.

The request is made without cookies or credentials and includes none of your data. As with any internet connection, GitHub (which hosts the file) receives your IP address and technical browser information; that is covered by [GitHub's privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

## Donation link

The popup has a link to Ko-fi for voluntary donations. It only opens if you click it, and from then on Ko-fi's privacy policy applies.

## Changes to this policy

If this policy changes, this page and the date above will be updated.

## Contact

Questions: open an issue at [github.com/ngalonsoc/omniskip-selectors/issues](https://github.com/ngalonsoc/omniskip-selectors/issues).
