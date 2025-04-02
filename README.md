# Proyecto: Gestión de Estudiantes

## Descripción
Este proyecto es una API REST desarrollada con Spring Boot para la gestión de estudiantes. Permite realizar operaciones CRUD sobre los estudiantes, incluyendo creación, consulta, actualización y eliminación.

## Funcionalidades
- Obtener todos los estudiantes
- Obtener un estudiante por ID
- Registrar un nuevo estudiante
- Actualizar un estudiante existente
- Eliminar un estudiante por ID

## Tecnologías Utilizadas
- **Spring Boot** (Framework principal)
- **Lombok** (Reducción de código repetitivo en POJOs)
- **Maven** (Gestión de dependencias)
- **Java 17** (Lenguaje de programación)

## Instalación y Ejecución
1. Clonar el repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   ```
2. Navegar al directorio del proyecto:
   ```bash
   cd mi-proyecto-spring-boot
   ```
3. Construir el proyecto con Maven:
   ```bash
   mvn clean install
   ```
4. Ejecutar la aplicación:
   ```bash
   mvn spring-boot:run
   ```

## Pruebas con Postman
### 1. Obtener todos los estudiantes
- **Método:** GET
- **URL:** `http://localhost:8080/api/estudiantes`

### 2. Obtener un estudiante por ID
- **Método:** GET
- **URL:** `http://localhost:8080/api/estudiantes/{id}`

### 3. Registrar un estudiante
- **Método:** POST
- **URL:** `http://localhost:8080/api/estudiantes`
- **Body (JSON):**
  ```json
  {
    "nombre": "Carlos",
    "apellido": "Lopez",
    "email": "carlos.lopez@example.com",
    "fechaNacimiento": "2002-06-15",
    "numeroInscripcion": "S003"
  }
  ```

### 4. Actualizar un estudiante
- **Método:** PUT
- **URL:** `http://localhost:8080/api/estudiantes/{id}`
- **Body (JSON):**
  ```json
  {
    "nombre": "Carlos",
    "apellido": "Lopez",
    "email": "carlos.lopez@example.com",
    "fechaNacimiento": "2002-06-15",
    "numeroInscripcion": "S003"
  }
  ```

### 5. Eliminar un estudiante
- **Método:** DELETE
- **URL:** `http://localhost:8080/api/estudiantes/{id}`
