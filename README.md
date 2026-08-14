# Events Docs

Documentación pública de las herramientas de [EventsMC](https://eventsmc.xyz), en un único sitio:

- **Events Whitelist** — gestiona la whitelist de tu servidor de Minecraft desde Discord.
- **Events Blacklist** — baneos compartidos y anónimos entre comunidades de Discord.

Está escrita para [Mintlify](https://mintlify.com): `docs.json` define la navegación (una pestaña
por bot) y cada página es un `.mdx`.

## Estructura

```
docs.json           navegación, tema y colores
favicon.svg
index.mdx           portada: elige bot
afiliados.mdx       programa de afiliados (común a los dos bots)
whitelist/          documentación de Events Whitelist
blacklist/          documentación de Events Blacklist
```

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
| `privacy` | Cómo se protege el origen de cada baneo |
| `commands` | Referencia de todos los comandos |
| `permissions` | Quién puede usar qué, y permisos que necesita el bot |
| `faq` | Preguntas frecuentes |
| `troubleshooting` | Problemas habituales y cómo resolverlos |
| `changelog` | Novedades |

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
