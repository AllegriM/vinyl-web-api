# API de Álbumes

Esta es una API simple en memoria que permite realizar operaciones básicas en una colección de álbumes. Puedes usar esta API para obtener una lista de álbumes, agregar nuevos álbumes y obtener información de un álbum específico según su ID.

## Instalación

1. Asegúrate de tener Go instalado en tu sistema. Puedes descargar Go desde [https://golang.org](https://golang.org) e instalarlo siguiendo las instrucciones adecuadas para tu plataforma.

2. Clona el repositorio de la API de álbumes desde GitHub ejecutando el siguiente comando:

``` git clone https://github.com/AllegriM/vinyl-web-api.git ```

3. Cambia al directorio del proyecto:

``` cd vinyl-web-api ```

4. Instala las dependencias del proyecto utilizando el comando `go get`:

``` go get -d ./... ```

## Uso

1. Inicia el servidor de la API ejecutando el siguiente comando:

``` go run main.go ```

2. La API estará disponible en `http://localhost:8080`.

## Endpoints

### Obtener todos los álbumes

``` GET /albums ```


Este endpoint devuelve una lista de todos los álbumes en formato JSON.

### Obtener un álbum por ID

``` GET /albums/:id ```

Este endpoint devuelve un álbum específico según el ID proporcionado. Reemplaza `:id` en la ruta con el ID del álbum deseado.

### Agregar un nuevo álbum


``` POST /albums ```

Este endpoint permite agregar un nuevo álbum. Debes proporcionar los datos del álbum en formato JSON en el cuerpo de la solicitud.

## Ejemplo de estructura de álbum

Aquí tienes un ejemplo de cómo se ve la estructura de un álbum en formato JSON:

``` json
{
    "id": "1",
    "title": "Blue Train",
    "artist": "John Coltrane",
    "price": 56.99
} ```

