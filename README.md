# Ichnos

![Status](https://img.shields.io/badge/status-en%20desarrollo-yellow)
![Backend](https://img.shields.io/badge/backend-Spring%20Boot-brightgreen)
![Frontend](https://img.shields.io/badge/frontend-React-blue)
![Database](https://img.shields.io/badge/database-SQLite-lightgrey)
![License](https://img.shields.io/badge/license-MIT-green)

***Sistema de gestión de tickets enfocado en trazabilidad, evidencias y análisis de soporte técnico.***

---

##  Descripción

**Ichnos** es una plataforma diseñada para documentar la ***huella completa*** de cada ticket dentro de un entorno de soporte técnico.

A diferencia de herramientas tradicionales, Ichnos registra no solo el resultado, sino ***todo lo que ocurre durante el proceso***:

- Intentos de contacto  
- Respuestas del cliente  
- Accesos remotos  
- Acciones técnicas  
- Evidencias (imágenes, archivos)  
- Solución y cierre  

Cada ticket se convierte en una ***línea de tiempo auditable***.

---

##  Problema que resuelve

En operaciones reales de soporte:

-  No hay trazabilidad detallada  
-  Se pierde información importante  
-  No se documentan intentos de contacto  
-  No hay evidencia estructurada  
-  Se depende de la memoria del técnico  

Esto genera errores, retrabajo y baja eficiencia.

---

##  Propuesta de valor

Ichnos introduce un enfoque basado en ***eventos***, donde cada acción queda registrada.

- Trazabilidad total  
- Evidencia documentada  
- Historial reutilizable  
- Mejora continua basada en datos  

---

##  Características

###  Timeline de eventos (core)

Cada ticket contiene un historial completo:

- Intento de contacto  
- Sin respuesta  
- Cliente responde  
- Acceso otorgado  
- Intervención técnica  
- Solución aplicada  
- Cierre  

---

###  Gestión de contactos

- Directorio por cliente y sede  
- Múltiples medios de contacto  
- Historial implícito de efectividad  

---

###  Clientes y sedes

- Multi-cliente  
- Multi-ubicación  
- Identificación clara mediante claves  

---

###  Equipos

- Registro de dispositivos  
- Asociación con tickets  
- Historial de incidencias  

---

###  Catálogos

- Estatus  
- Problemas  
- Causas  
- Medios de contacto  
- Medios de acceso  
- Tipos de evento  

---

###  Evidencias

- Adjuntos por evento  
- Almacenamiento seguro (OneDrive local)  
- Sin exposición pública  

---

###  Transferencias

- Registro de cambios de responsabilidad  
- Trazabilidad entre áreas  

---

##  Tecnologías

- **Backend:** Spring Boot  
- **Frontend:** React  
- **Base de datos:** SQLite  
- **Storage:** OneDrive (sin enlaces públicos)  

---

## Arquitectura
```text
.
├── backend/                # API REST con Spring Boot
│   ├── controller/         # Endpoints y manejo de peticiones
│   ├── service/            # Lógica de negocio
│   ├── repository/         # Persistencia de datos (JPA)
│   ├── entity/             # Entidades de base de datos
│   ├── dto/                # Objetos de transferencia de datos
│   └── config/             # Configuraciones del sistema
├── frontend/               # Interfaz de usuario
│   └── react-app/          # SPA con React.js
└── README.md
\
```

---

## Flujo de trabajo

1. Crear ticket  
2. Seleccionar cliente / sede / contacto  
3. Registrar intentos de contacto  
4. Documentar respuesta  
5. Ejecutar intervención técnica  
6. Adjuntar evidencia  
7. Resolver y cerrar  

Todo queda registrado como eventos.

---

## Seguridad

- Ejecución local (offline-first)  
- Sin exposición a internet  
- Manejo seguro de archivos  
- Preparado para autenticación futura  

---

##  Roadmap

- [x] Definición de arquitectura  
- [ ] Backend (Spring Boot)  
- [ ] Modelo de datos completo  
- [ ] API REST  
- [ ] Frontend (React)  
- [ ] Timeline visual  
- [ ] Módulo de evidencias  
- [ ] Dashboard  

---

##  Demo

***Próximamente***

---

##  Filosofía

> “No se trata solo de resolver tickets,  
> sino de entender todo lo que ocurrió en ellos
> para tener herramientas para el futuro.”

---

##  Estado

- En desarrollo activo  
- Arquitectura definida  

---

## Autor

Proyecto desarrollado como solución a problemas reales de soporte técnico, con enfoque en trazabilidad, control y mejora continua.

---

## Licencia

MIT License

---

## Contribuciones

- Puedes abrir un issue  
- Proponer mejoras  
- Compartir ideas  

---
