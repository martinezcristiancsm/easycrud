# Guía para Correr la Aplicación Java Spring Boot

## Requisitos

- **Java 17 o superior**: Verifica con `java -version`.
- **Maven**: Verifica con `mvn -v`.

## Clonar el Repositorio

1. Clona el repositorio:

   ```bash
   git clone easycrud

    Navega al directorio del proyecto:

    cd easycrud

Configuración del Puerto, username y pw de la db

El puerto de la aplicación está configurado en src/main/resources/application.properties. Cambia los siguientes valores por tus valores de preferencia:

spring.datasource.url=jdbc:mysql://localhost:{puerto a usar}/easycrud
spring.datasource.username={nombre de usuario}
spring.datasource.password={password}

Construir y Correr la Aplicación

    Construye la aplicación:
    
mvn clean install

Córrela:

    mvn spring-boot:run

Accede a la aplicación en http://localhost:8080 (o el puerto que hayas configurado).
