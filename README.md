#  Sistema de Gestión Integral

## Descripción del Proyecto
Este proyecto tiene como objetivo desarrollar un **Sistema de Gestión Integral** que permite administrar usuarios, procesos y recursos de manera automatizada.  
A través del modelado con **UML (Lenguaje Unificado de Modelado)**, se diseñaron los componentes esenciales del sistema, sus interacciones y el comportamiento de los objetos.

El desarrollo se basa en los principios de **orientación a objetos**, **modularidad** y **escalabilidad**, buscando un diseño mantenible y adaptable a distintas necesidades.

---

##  Características Principales
- Registro y autenticación de usuarios.  
- Gestión de roles y permisos.  
- Creación, ejecución y control de procesos internos.  
- Generación de reportes automatizados.  
- Control de estados y eventos de usuarios y procesos.  
- Persistencia de datos con base de datos relacional.  

---

##  Diagramas UML Incluidos

###  Diagramas de Casos de Uso
Muestran las interacciones entre los actores principales y el sistema.

### 🕓 Diagramas de Secuencia (12 en total)
Describen la comunicación temporal entre los actores y los objetos del sistema.  
Cada interacción incluye:
- Actor (persona o sistema externo).  
- Mensajes con sus **métodos** y **respuestas**.  
- Activaciones y desactivaciones.  

Ejemplo:
| Actor | Método | Respuesta |
|--------|---------|------------|
| Usuario | `iniciarSesion()` | `validarCredenciales()` |
| Sistema | `consultarDatosUsuario()` | `retornarDatos()` |

###  Diagramas de Estado
Representan los cambios de estado de los objetos durante su ciclo de vida.  
Los dos más importantes son:
1. **Estado del Usuario:** Registrado → Activo → Inactivo → Eliminado.  
2. **Estado del Proceso:** Pendiente → En ejecución → Completado → Cancelado.  

###  Diagrama de Clases
Define la estructura principal del sistema con relaciones de herencia, agregación y asociación:

| Clase | Rol | Relación |
|--------|------|-----------|
| `Usuario` | Gestiona autenticación y datos personales | Hereda de `Persona` |
| `Administrador` | Supervisa el sistema y usuarios | Agregación con `Usuario` |
| `Proceso` | Representa operaciones internas | Asociación con `Usuario` |
| `Reporte` | Genera informes automáticos | Depende de `Proceso` |

---

## ⚙️ Tecnologías Utilizadas
- **Lenguaje:** JavaScript / PHP 
- **Base de datos:** PostgreSQL / SQL/ Supabase  
- **Herramientas UML:** StarUML, Draw.io  
- **IDE:** Visual Studio   
- **Control de versiones:** GitHub  

