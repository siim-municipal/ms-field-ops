# 📱 MS Field Operations (Operaciones de Campo)

Microservicio diseñado para soportar las actividades de **inspección, verificación y notificación** en campo. Sirve como backend para las aplicaciones móviles de los inspectores municipales.

![Geo](https://img.shields.io/badge/Data-Geospatial-green)
![Mobile Backend](https://img.shields.io/badge/Role-BFF-blue)

## 📋 Funcionalidades

* **Asignación de Visitas:** Rutas de trabajo para notificadores/inspectores.
* **Levantamiento de Actas:** Registro digital de inspecciones (Obras, Comercios).
* **Evidencia Fotográfica:** Carga y almacenamiento de fotos de predios/licencias.
* **Geolocalización:** Registro de coordenadas GPS de la visita.

## 🛠️ Integración

* Consume **MS Padrón** para obtener direcciones y datos del predio.
* Reporta a **MS Tesorería** si se generan multas o recargos en sitio.

## ⚙️ Requisitos

Este servicio suele requerir almacenamiento de archivos (S3, MinIO o FileSystem local) para las evidencias.

| Variable | Descripción |
| :--- | :--- |
| `URL_BD_FIELDOPS` | Base de datos operativa |
| `STORAGE_TYPE` | `LOCAL` o `S3` |
| `STORAGE_PATH` | Ruta para guardar evidencias fotográficas |

---
