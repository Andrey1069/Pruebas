# Gestión de Productos Reactivo

Proyecto básico para aprender **Spring Boot**, **Spring Security**, **programación reactiva con WebFlux**, **internacionalización (i18n)** en 3 idiomas (español, inglés, francés), y conexión con **MongoDB** usando operaciones CRUD.

## Tecnologías Usadas

- Java 17
- Spring Boot 3.x
- Spring WebFlux (reactivo)
- Spring Security
- Spring Data Reactive MongoDB
- Internacionalización (i18n)
- Postman (para pruebas)
- Lombok

## Internacionalización

Endpoint de prueba:
GET /api/products/mensaje?lang=es | en | fr


## Seguridad

- Autenticación básica (HTTP Basic)
- Usuario: 'usuario'
- Contraseña: 'clave123'

## Endpoints CRUD (Protegidos)

| Método | Endpoint | Descripción |
|---|---|---|
| GET | `/api/products` | Lista todos los productos |
| POST | `/api/products` | Crear un nuevo producto |
| GET | `/api/products/{id}` | Buscar producto por ID |
| PUT | `/api/products/{id}` | Actualizar producto por ID |
| DELETE | `/api/products/{id}` | Eliminar producto por ID |

## Pruebas con Postman

1. Usa autenticación básica con el usuario y clave.
2. Prueba el CRUD y el endpoint `/mensaje?lang=fr`.

## Requisitos para ejecutar

- Java 17
- Maven 3.8+
- MongoDB local (en `localhost:27017`)

## Cómo correr el proyecto

```bash
# Clonar el repositorio
git clone https://github.com/Andrey1069/api-rest.git

# Entrar al proyecto
cd api-rest

# Ejecutar el proyecto
./mvnw spring-boot:run

