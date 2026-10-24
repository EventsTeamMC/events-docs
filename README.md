# Events Docs

Documentación pública de las herramientas de [EventsMC](https://eventsmc.xyz), en un único sitio:

- **Panel de control** — instancias, eventos, equipo, Events+ y launchers de marca.
- **Events Whitelist** — gestiona la whitelist de tu servidor de Minecraft desde Discord.
- **Events Blacklist** — baneos compartidos y anónimos entre comunidades de Discord.
- **Events BOT** — un bot de Discord propio, con tu nombre y tus colores, alojado por Events.

Está escrita para [Mintlify](https://mintlify.com): `docs.json` define la navegación (una pestaña
por producto) y cada página es un `.mdx`.

## Estructura

```
docs.json           navegación, tema y colores
favicon.png
images/
index.mdx           portada
afiliados.mdx       programa de afiliados
panel/              panel de control
whitelist/          Events Whitelist
blacklist/          Events Blacklist
bot/                Events BOT
```

### Panel de control

| Página | Contenido |
|---|---|
| `introduction` | Qué es el panel y cómo se entra |
| `session` | Sesión e idiomas |
| `instances` | Instancias del launcher |
| `events` | Eventos y calendario |
| `team` | Equipo y studios |
| `webhooks` | Webhooks |
| `files` | Archivos públicos |
| `bots` | Bots de Discord desde el panel |
| `hosting` | Servidores de juego |
| `ultra` | Events+ Ultra |
| `launchers` | Launchers de marca y dominio propio |
| `evac-plus` | EVAC+ en directo |
| `changelog` | Novedades |

### Events Whitelist

| Página | Contenido |
|---|---|
| `introduction` | Qué es el bot y qué puedes hacer con él |
| `quickstart` | Puesta en marcha en 5 minutos |
| `guide` | Guía completa: de la primera whitelist al servidor sincronizado |
| `how-it-works` | El flujo de registro visto por el jugador |
| `roles` | Roles requeridos, bloqueados, concedidos y retirados |
| `logs` | Canales de logs del servidor y por whitelist |
| `export` | Formatos de exportación y cuál usar |
| `minecraft-plugin` | Plugin oficial de Minecraft |
| `api` | API REST + WebSocket para integraciones propias |
| `commands` | Referencia de todos los comandos |
| `permissions` | Quién puede usar qué, y permisos que necesita el bot |
| `faq` | Preguntas frecuentes |
| `troubleshooting` | Problemas habituales y cómo resolverlos |
| `changelog` | Novedades versión a versión |

### Events Blacklist

| Página | Contenido |
|---|---|
| `introduction` | Qué es el bot y qué problema resuelve |
| `quickstart` | Puesta en marcha en 5 minutos |
| `guide` | Guía completa: del setup a la política de moderación |
| `how-it-works` | El ciclo de vida de un baneo, de punta a punta |
| `alerts` | Cuándo avisa el bot, y cómo ajustarlo |
| `auto-ban` | Baneo automático: cuándo activarlo y con qué umbral |
| `privacy` | Cómo se protege el origen de cada baneo y Events Database |
| `commands` | Referencia de todos los comandos |
| `permissions` | Quién puede usar qué, y permisos que necesita el bot |
| `faq` | Preguntas frecuentes |
| `troubleshooting` | Problemas habituales y cómo resolverlos |
| `changelog` | Novedades |

### Events BOT

| Página | Contenido |
|---|---|
| `introduction` | Qué es |
| `quickstart` | De la compra al bot en línea |
| `configurar` | `/configurar`: apariencia, presencia, módulos, textos y tickets |
| `modules` | Los módulos |
| `panel` | Gestión desde el panel |
| `hosting` | Lo que se hace desde hosting.eventsmc.xyz |
| `faq` | Preguntas frecuentes |

## Desarrollo local

```bash
npm i -g mint
mint dev
```

## Publicar

Los cambios en `main` se publican automáticamente a través de la integración de Mintlify con
GitHub.

## Añadir un producto nuevo

1. Crea la carpeta con sus `.mdx`.
2. Añade una pestaña más en `navigation.tabs` de `docs.json`.
3. Enlázalo desde `index.mdx`.
