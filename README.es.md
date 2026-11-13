<div align="center">

# BustaSQL

### Un IDE de bases de datos. Todos los motores. En tu equipo.

**Un IDE de escritorio moderno para Microsoft SQL Server, Azure SQL Database, MySQL/MariaDB y PostgreSQL, con comparación de esquemas y datos, planes de ejecución, edición directa en la cuadrícula y asistente de IA.**

[![Última versión](https://img.shields.io/github/v/release/sensodent/BustaSQL-Releases?label=%C3%BAltima%20versi%C3%B3n&color=ef6257)](https://github.com/sensodent/BustaSQL-Releases/releases/latest)
![Windows](https://img.shields.io/badge/Windows-x64-242424?logo=windows)
![Bases de datos](https://img.shields.io/badge/SQL%20Server%20%C2%B7%20Azure%20SQL%20%C2%B7%20MySQL%20%C2%B7%20PostgreSQL-242424)
![Gratis](https://img.shields.io/badge/Descarga-Gratis-242424)

**[⬇ Descargar BustaSQL para Windows](https://github.com/sensodent/BustaSQL-Releases/releases/latest)**

[🌐 English](README.md) · **🇪🇸 Español**

</div>

---

## Conoce BustaSQL

**BustaSQL** es un IDE de bases de datos de escritorio que se ejecuta íntegramente en tu equipo: un servidor local que solo escucha en `127.0.0.1` y una interfaz rápida en su propia ventana. Usa tu red y tu VPN corporativa, y **nunca envía tu SQL ni tus datos a servidores de BustaSQL**: no existen.

Explora miles de tablas, escribe consultas con IntelliSense real, compara esquemas y datos entre entornos y edita los resultados directamente en la cuadrícula. **Sin ir saltando entre herramientas distintas para cada motor.**

<!-- Capturas: añade assets/bustasql-editor.png y assets/bustasql-compare.png y descomenta.
![Editor de consultas de BustaSQL](assets/bustasql-editor.png)
![Schema Compare de BustaSQL](assets/bustasql-compare.png)
-->

## ¿Qué incluye?

| Función | Qué obtienes |
| --- | --- |
| **Motores** | SQL Server 2008 y posteriores, Azure SQL Database, MySQL 8 / MariaDB y PostgreSQL 10+, también a través de **túneles SSH** con verificación de huella. |
| **Autenticación** | Inicios de sesión SQL, **Microsoft Entra ID interactivo (MFA)**, Entra *Default* (Azure CLI), Service Principal, access token y Windows NTLM. |
| **Explorador** | Árbol virtualizado con carga diferida: esquemas, tablas, columnas, claves, índices, triggers, inicios de sesión, usuarios y roles, con scripts CREATE/ALTER/DROP/SELECT/INSERT/EXEC. |
| **Editor de consultas** | Editor Monaco con IntelliSense basado en metadatos reales (alias, CTE, otras BD), snippets, formateo, ir a definición y validación de sintaxis sin ejecutar. |
| **Ejecución** | Todo, selección o instrucción actual; lotes `GO`; varios resultados; cancelación por pestaña; indicador de transacción abierta con COMMIT/ROLLBACK; **ejecutar una consulta en varias bases de datos a la vez**. |
| **Resultados** | Cuadrícula virtualizada con *back-pressure* real para millones de filas, filtros por columna, copiar como tabla (se pega en Teams, Outlook, Excel), visores JSON/XML y exportación CSV/TSV/JSON/Excel. |
| **Edición directa** | Edita celdas, pega rangos, inserta y borra filas, revisa el SQL y aplícalo en una transacción con detección de conflictos. |
| **Schema Compare** | Comparación semántica de tablas, claves, índices, vistas, procedimientos, funciones y más, con script de sincronización transaccional, ordenado por dependencias y con avisos de pérdida de datos. |
| **Data Compare** | Comparación por lotes en streaming con claves compuestas y filtros WHERE, vista lado a lado y scripts INSERT/UPDATE/DELETE. |
| **Planes de ejecución** | Planes estimados y reales, costes, advertencias, índices sugeridos, estadísticas IO/TIME y exportación `.sqlplan`. |
| **Diseñador de tablas** | Crea y modifica tablas con scripts revisables, incluido reordenar columnas arrastrando sin perder datos. |
| **Asistente IA** | Chat y edición en línea con **Claude Code**, **Codex** o **Cursor** (los CLIs instalados en tu equipo, con tu cuenta): explora tu esquema real, escribe consultas y las ejecuta con tu permiso. |
| **Seguridad** | Entornos (Desarrollo / Pruebas / **Producción**, con borde rojo y confirmaciones reforzadas) y conexiones de solo lectura. |

## Empieza

1. **[Descarga el instalador más reciente para Windows](https://github.com/sensodent/BustaSQL-Releases/releases/latest)** (`BustaSQL-Setup-X.Y.Z.exe`).
2. Ejecútalo. Se instala para tu usuario, **sin permisos de administrador** y **sin Node.js**.
3. Abre BustaSQL, pulsa **+** en el explorador y crea una conexión.

> El instalador todavía no está firmado digitalmente. Windows SmartScreen puede mostrar *«Windows protegió su PC»*: pulsa **Más información → Ejecutar de todas formas** solo si lo has descargado de este repositorio.

BustaSQL es **gratuito**. Las cuentas, suscripciones y límites de uso de los proveedores de IA son **independientes** y solo se usan si activas el asistente.

## Privacidad, credenciales y actualizaciones

- BustaSQL se ejecuta en local. Las conexiones van directamente de tu equipo a tus servidores de bases de datos.
- Las contraseñas se guardan en el **Administrador de credenciales de Windows** (DPAPI), nunca en texto plano. La configuración se puede exportar **sin secretos**.
- Lo único que sale de tu equipo hacia un tercero es el contexto que compartes con el **asistente de IA**, que se envía al proveedor que elijas (Anthropic, OpenAI o Cursor) con tu propia cuenta.
- Tus conexiones, historial y consultas guardadas están en `%LOCALAPPDATA%\BustaSQL` y se conservan al desinstalar.
- BustaSQL busca actualizaciones en este repositorio al arrancar y cada 4 horas, comprueba la descarga con el checksum SHA-512 de `latest.yml` y te pide reiniciar.

## Soporte y comunidad

- [Informar de un error, preguntar o proponer una mejora](https://github.com/sensodent/BustaSQL-Releases/issues/new/choose)
- [FAQ](FAQ.md) · [Soporte](SUPPORT.md) · [Seguridad](SECURITY.md)
- [Contribuir](CONTRIBUTING.md) · [Código de conducta](CODE_OF_CONDUCT.md) · [Accesibilidad](ACCESSIBILITY.md) · [Aviso de licencia](LICENSE)

## Descarga y estado del proyecto

**[Última versión](https://github.com/sensodent/BustaSQL-Releases/releases/latest)** · [Todas las versiones](https://github.com/sensodent/BustaSQL-Releases/releases)

- **Instalador disponible:** Windows x64.
- **Código fuente:** actualmente privado. Este repositorio público distribuye los instaladores y los archivos de actualización, no el código.
- BustaSQL es un proyecto independiente y no está afiliado a Microsoft, Oracle, PostgreSQL Global Development Group, MariaDB, Anthropic, OpenAI, Cursor ni a los demás productos mencionados.

---

<div align="center">

**Consulta. Compara. Despliega.**

**[Descargar BustaSQL](https://github.com/sensodent/BustaSQL-Releases/releases/latest)** · [Read in English](README.md)

</div>
