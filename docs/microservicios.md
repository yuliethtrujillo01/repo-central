```
# inventario de microservicios (equipo)

> Mantener en actualizacion. Toda fila sin responsable o sin URL válida se considera **incompleta**.

## tabla resumen

| Servicio (ID)  | Descripción breve                       | Repo URL                               | Base URL (EC2)             | Swagger UI                            | Responsable               | Estado      |
| -------------- | --------------------------------------- | -------------------------------------- | -------------------------- | ------------------------------------- | ------------------------- | ----------- |
| curso-service  | Autenticación JWT (login/refresh)       | https://github.com/<org>/<repo-auth>   | http://<ip-o-dominio>:8081 | http://<ip-o-dominio>:8081/swagger-ui | Nombre Apellido (@github) | En progreso |
| ova-service    | CRUD OVA/módulos/lecciones              | https://github.com/<org>/<repo-ova>    | http://<ip-o-dominio>:8082 | http://<ip-o-dominio>:8082/swagger-ui | Nombre Apellido (@github) | En progreso |
| RabbitMQ-service  | Gestión de assets (pdf/img/video-url)   | https://github.com/<org>/<repo-asset>  | http://<ip-o-dominio>:8083 | http://<ip-o-dominio>:8083/swagger-ui | Nombre Apellido (@github) | Pendiente   |

> **Ejemplo de llenado real:**  
> - “Base URL (EC2)”: usar IP pública o dominio del servidor.  
> - “Estado”: Pendiente / En progreso / Listo.

---

## detalle por servicio (plantilla)

### <servicio>-service
- **Responsable:** Nombre Apellido (@github)  
- **Repositorio:** https://github.com/<org>/<repo-del-servicio>  
- **Base URL (EC2):** http://<ip-o-dominio>:<puerto>  
- **Swagger UI:** http://<ip-o-dominio>:<puerto>/swagger-ui  
- **Entidades principales:**  
  - `<EntidadPrincipal>` (campos clave: …)  
- **Endpoints mínimos:**  
  - `POST /api/<recurso>`  
  - `GET /api/<recurso>`  
  - `GET /api/<recurso>/{id}`  
  - `PUT /api/<recurso>/{id}`  
  - `DELETE /api/<recurso>/{id}`  
- **Checklist de verificación (semanal):**  
  - [ ] Compila y arranca local  
  - [ ] `/actuator/health` **UP** en local  
  - [ ] Swagger accesible en EC2  
  - [ ] Push diario con commits significativos  
  - [ ] Historia/tarea en Jira: **En progreso** → **Terminado** al finalizar

---

## responsables (vista rápida)

| Rol | Nombre | Usuario GitHub | Observaciones |
|---|---|---|---|
| Scrum Master | Nombre Apellido | @usuario | — |
| DevOps | Nombre Apellido | @usuario | EC2, puertos, dominios |
| QA | Nombre Apellido | @usuario | Revisión básica de respuestas |
| Autor(es) de servicio(s) | Nombre Apellido | @usuario | Indicar cuál servicio |

---

## notas de la semana
- Fecha: AAAA-MM-DD  
- Cambios relevantes:  
  - …  
- Bloqueos/riesgos:  
  - …
```
