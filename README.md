# care-relay-r1

Servidor de relay de mensajes en tiempo real construido con Node.js y Socket.IO.

## Alcance actual

Esta versión provee:
- Relay de mensajes genéricos entre clientes (`relay_message`)
- Mensajes privados (`private_message`)
- Gestión de salas (`join_room`, `room_message`, `leave_room`)
- Broadcast de datos (`broadcast_data`)
- Actualización de metadata de usuarios (`update_metadata`)
- Obtención de usuarios y salas (`get_connected_users`, `get_rooms_info`)
- Monitoreo básico con los endpoints `/stats` y `/health`

> **NOTA IMPORTANTE**:
> Esta versión de care-relay-r1 está alineada 100% con este documento.
> No incluye nickname, autenticación, buffers circulares, canales semánticos ni persistencia de mensajes.
> Solo incluye relay de mensajes genéricos, rooms y monitoreo de conexiones, todo en memoria, sin seguridad ni validaciones estrictas.
> Para agregar nuevas features, crear PRs específicos referenciando este documento como base de comparación.

## Features No Implementadas / Fuera de Alcance
- Gestión de nickname de usuarios
- Autenticación y autorización
- Persistencia de mensajes o usuarios
- Buffers circulares o colas de mensajes
- Seguridad avanzada y cifrado
- API REST extendida (por ejemplo `/api/clients`, `/api/rooms`)
