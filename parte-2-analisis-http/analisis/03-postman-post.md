# Análisis 3: Petición POST con Postman

## Configuración de la petición

Para realizar la prueba se utilizó Postman para enviar una petición HTTP mediante el método **POST** a la API pública de pruebas JSONPlaceholder.

| Dato             | Valor                                        |
| ---------------- | -------------------------------------------- |
| Método HTTP      | POST                                         |
| URL              | `https://jsonplaceholder.typicode.com/posts` |
| Content-Type     | `application/json`                           |
| Formato del Body | JSON (raw)                                   |

El cuerpo enviado en la petición fue:

```json
{
  "title": "Laboratorio Programacion Web",
  "body": "Analisis de peticiones HTTP con Postman.",
  "userId": 1
}
```

## Respuesta recibida

La petición fue procesada correctamente por el servidor y se obtuvo el código de estado **201 Created**, indicando que la solicitud fue aceptada y que la API simuló correctamente la creación del recurso.

La respuesta recibida incluyó los datos enviados junto con un identificador asignado:

```json
{
  "title": "Laboratorio Programacion Web",
  "body": "Analisis de peticiones HTTP con Postman.",
  "userId": 1,
  "id": 101
}
```

El campo `id` permite identificar el recurso generado por la API. JSONPlaceholder es una API de pruebas, por lo que la creación del recurso es simulada y no representa necesariamente un almacenamiento permanente en una base de datos real.

## Headers relevantes

El header principal configurado en la petición fue:

| Header       | Valor              | Significado                                                       |
| ------------ | ------------------ | ----------------------------------------------------------------- |
| Content-Type | `application/json` | Indica que el cuerpo de la petición está enviado en formato JSON. |

La respuesta del servidor también indicó que el contenido recibido correspondía a una respuesta JSON.

## Resultado de los tests

Se agregaron dos pruebas automáticas en Postman para verificar que la petición se procesara correctamente.

| Test                          | Resultado |
| ----------------------------- | --------- |
| Status 201 Created            | **PASS**  |
| Respuesta incluye id asignado | **PASS**  |

El primer test verificó que el código de respuesta fuera **201**. El segundo comprobó que la respuesta incluyera la propiedad `id` y que el título recibido coincidiera con `"Laboratorio Programacion Web"`. Ambos tests fueron ejecutados correctamente y aparecieron en verde en **Test Results**.

## Diferencias entre GET y POST

La principal diferencia entre las peticiones **GET** y **POST** está en su propósito. GET se utiliza principalmente para solicitar información de un recurso, como ocurrió al consultar `/posts/1`, mientras que POST permite enviar información al servidor para crear o procesar un nuevo recurso. En la petición GET analizada anteriormente no fue necesario enviar un cuerpo con datos, mientras que en la petición POST se envió un cuerpo en formato JSON con los campos `title`, `body` y `userId`. Además, la consulta GET devolvió un código **200 OK**, mientras que la petición POST realizada correctamente devolvió **201 Created**.

## Conclusión

La prueba realizada con Postman permitió comprobar el funcionamiento de una petición POST hacia una API REST pública. La solicitud fue enviada correctamente en formato JSON y el servidor respondió con un código **201 Created** junto con un identificador para el recurso generado. Los dos tests configurados en Postman se ejecutaron correctamente, confirmando tanto el código de respuesta como la presencia de los datos esperados. La actividad permitió identificar las diferencias entre GET y POST y comprender cómo se utilizan los métodos HTTP para solicitar y enviar información a una API.
