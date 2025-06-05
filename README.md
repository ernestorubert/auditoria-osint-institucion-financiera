# Auditoría de Seguridad OSINT: Exposición Crítica de Logs y Credenciales en Entorno Financiero

Este repositorio contiene un informe técnico **anonimizado** generado tras una auditoría de seguridad web mediante técnicas OSINT (Open Source Intelligence), enfocada en identificar brechas de configuración en una institución financiera del sector préstamos personales.

## 📄 Descripción del proyecto

Durante una evaluación proactiva realizada en junio de 2025, se identificó una **vulnerabilidad crítica** que permitía el acceso público a múltiples archivos de log (.log) expuestos en la infraestructura web de la entidad. Estos archivos contenían datos personales, registros de consultas a sistemas externos, credenciales internas y acceso sin restricción a herramientas administrativas como phpMyAdmin.

El hallazgo evidencia cómo errores comunes de configuración pueden traducirse en un **riesgo severo para la confidencialidad, integridad y disponibilidad** de la información, así como en posibles sanciones legales por incumplimiento de normativas de protección de datos.

## 🧰 Herramientas y técnicas utilizadas

- **Google Dorking** (`site:ejemplo.com filetype:log "password"`)
- **curl / wget** para obtener evidencia sin generar tráfico web adicional
- Análisis manual de logs
- Evaluación del servidor web y navegación por directorios
- OSINT y principios de auditoría ética

## 📌 Principales hallazgos

- Exposición pública de archivos `.log` sin autenticación
- Presencia de información sensible: nombres, direcciones, RFC, tokens de API, rutas internas
- Acceso a interfaces administrativas como phpMyAdmin sin protección
- Posibles violaciones a la Ley Federal de Protección de Datos Personales (LFPDPPP - México)

## ⚠️ Riesgos identificados

- Robo de identidad y fraude financiero
- Ataques dirigidos mediante ingeniería social o escalación de privilegios
- Compromiso de sistemas internos y servicios backend
- Reputación organizacional y sanciones legales

## ✅ Recomendaciones propuestas

- Medidas inmediatas: bloqueo de rutas sensibles, eliminación de logs públicos
- Corto plazo: auditoría de servidores, restricción de accesos administrativos por IP
- Mediano plazo: monitoreo automatizado con herramientas como OWASP ZAP, nikto, nuclei
- Políticas internas: hardening, control de logs, capacitación continua

## 📂 Contenido del repositorio

- [`reporte-auditoria-anonimizado.pdf`](./Auditoría%20de%20Seguridad%20OSINT%20Exposición%20Crítica%20de%20Logs%20y%20Credenciales%20en%20Entorno%20Financiero.pdf) – Informe completo y censurado
- Este `README.md` – Presentación general del caso técnico

## 📜 Licencia y uso

Este contenido se publica **con fines educativos y profesionales**.  
El objetivo es mostrar capacidades en **auditoría de seguridad, OSINT y buenas prácticas DevSecOps**.

---

### 🧑‍💻 Autor

**Ernesto Gamaliel Ruiz Rubert**  
[LinkedIn](https://www.linkedin.com/in/rubert-gamaliel/)  | [GitHub](https://github.com/ernestorubert)

