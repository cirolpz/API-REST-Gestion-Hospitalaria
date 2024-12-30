
# API REST para Gestión Hospitalaria 🚑

Este proyecto es una API REST diseñada para gestionar los datos de médicos, usuarios y pacientes en un entorno hospitalario. Se implementan principios de diseño de software, buenas prácticas de programación, y herramientas modernas para garantizar la calidad, seguridad y escalabilidad de la aplicación.

----------

## 📋 Funcionalidades principales

-   **Gestión de médicos**: Registro, actualización, y consulta de médicos disponibles.
-   **Gestión de usuarios y pacientes**: Administración de datos personales y seguimiento médico.
-   **Reservas de consultas**: Gestión eficiente de citas médicas, incluyendo asignación automática de médicos.

----------

## 🛠️ Tecnologías utilizadas

-   **Framework**: Spring Boot
-   **Base de datos**: MySQL (o in-memory para pruebas)
-   **Autenticación**: JSON Web Tokens (JWT)
-   **Documentación**: OpenAPI (SpringDoc)
-   **Construcción**: Maven
-   **Pruebas**: JUnit y pruebas automatizadas con base de datos in-memory

----------

## 🌟 Características avanzadas

1.  **Principios SOLID**: El diseño del sistema sigue los principios SOLID para mejorar la mantenibilidad y la escalabilidad.
2.  **Separación de lógica de negocio**: Uso del patrón Service para mantener el código limpio y modular.
3.  **Validaciones robustas**: Validación de datos con anotaciones como `@Valid`, personalización con `@JsonAlias`, y manejo de formatos de fechas.
4.  **Documentación profesional**:
    -   Generada con SpringDoc y OpenAPI Initiative.
    -   Incluye personalización para integrar JWT en la documentación interactiva.
5.  **Pruebas automatizadas**:
    -   Configuración de bases de datos de prueba.
    -   Verificación de casos de uso comunes (200, 400) y lógica de negocio.
6.  **Despliegue preparado**: Variables de entorno y posibilidad de empaquetar como `.war` o imagen nativa con GraalVM.

----------

## 🚀 Cómo ejecutar

### Prerrequisitos

-   **Java** 17 o superior.
-   **Maven** para construir el proyecto.
-   **MySQL** para la base de datos (o usar la configuración de in-memory para pruebas).

### Pasos para ejecutar

1.  Clona este repositorio:
    
    bash
    
    Copiar código
    
    `git clone https://github.com/tu-usuario/api-gestion-hospitalaria.git  
    cd api-gestion-hospitalaria` 
    
2.  Configura las variables de entorno:
    -   Base de datos:
        
        bash
        
        Copiar código
        
        `export DB_URL=jdbc:mysql://localhost:3306/hospital  
        export DB_USER=usuario  
        export DB_PASSWORD=contraseña` 
        
    -   JWT:
        
        bash
        
        Copiar código
        
        `export JWT_SECRET=tu-secreto  
        export JWT_EXPIRATION=3600000` 
        
3.  Construye el proyecto con Maven:
    
    bash
    
    Copiar código
    
    `mvn clean install` 
    
4.  Ejecuta la aplicación:
    
    bash
    
    Copiar código
    
    `java -jar target/api-gestion-hospitalaria-0.0.1.jar` 
    

----------

## 📘 Documentación de la API

-   Accede a la documentación interactiva en:
    
    bash
    
    Copiar código
    
    `http://localhost:8080/swagger-ui.html` 
    

----------

## 📦 Compilación y despliegue

-   **Construcción**:  
    Genera un archivo `.war` para despliegue en servidores:
    
    bash
    
    Copiar código
    
    `mvn package` 
    
-   **Despliegue nativo**:  
    Crea una imagen nativa con GraalVM:
    
    bash
    
    Copiar código
    
    `mvn -Pnative clean package`
