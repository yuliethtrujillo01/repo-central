+# inventario de microservicios (equipo)

> Mantener en actualizacion. Toda fila sin responsable o sin URL válida se considera **incompleta**.

## tabla resumen

| Servicio (ID)  | Descripción breve                       | Repo URL                               | Base URL (EC2)             | Swagger UI                            | Responsable               | Estado      |
| -------------- | --------------------------------------- | -------------------------------------- | -------------------------- | ------------------------------------- | ------------------------- | ----------- |
| curso-service  |  CRUD curso/módulos/lecciones        | https://github.com/alejandrobarco01-coder/CURSO-SERVICE  | http://<ip-o-dominio>:8081 | http://<ip-o-dominio>:8081/swagger-ui | Alejandro Barco (alejandrobarco01-coder) | En progreso |
| ova-service    | CRUD OVA/módulos/lecciones              | https://github.com/esteban429/ova-service:v1.0.0   | http://<ip-o-dominio>:8082 | http://<ip-o-dominio>:8082/swagger-ui | Jaime Jurado (esteban429) | En progreso |
| RabbitMQ-service  | Comunicacion entre microservicios   | https://github.com/yuliethtrujillo01/RabbitMQ.git  | http://<ip-o-dominio>:8083 | http://<ip-o-dominio>:8083/swagger-ui | Yulieth Trujillo (yuliethtrujillo01) | En progreso   |

> **Ejemplo de llenado real:**  
> - “Base URL (EC2)”: usar IP pública o dominio del servidor.  
> - “Estado”: Pendiente / En progreso / Listo.

---

## detalle por servicio (plantilla)

### (curso-service)-service
- **Responsable:** Alejandro Barco (alejandrobarco01-coder) 
- **Repositorio:** https://github.com/alejandrobarco01-coder/CURSO-SERVICE  
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

  ### (ova-service)-service
- **Responsable:** Jaime Jurado (esteban429) 
- **Repositorio:** https://github.com/esteban429/ova-service:v1.0.0
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
| Scrum Master | Yulieth Trujillo | yuliethtrujillo01 | entrenador o guía del equipo |
| DevOps | Sara Malaver | saramalaver01-cpu | EC2, puertos, dominios |
| QA | Alejandro Barco | alejandrobarco01-coder | Revisión básica de respuestas |
| Autor(es) de servicio(s) | Jaime Jurado | esteban429 | Indicar cuál servicio |

---

## notas de la semana
- Fecha: AAAA-MM-DD  
- Cambios relevantes:  
  - …  
- Bloqueos/riesgos:  
  - …

