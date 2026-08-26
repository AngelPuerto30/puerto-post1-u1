# Análisis 2: Petición GET — API REST JSONPlaceholder

## Información general

| Dato | Valor |
|---|---|
| URL | https://jsonplaceholder.typicode.com/posts/1 |
| Método | GET |
| Código de estado | 200 OK |

## Headers de Request

| Header | Valor |
|---|---|
| Host | [jsonplaceholder.typicode.com] |
| User-Agent | [Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/151.0.0.0 Safari/537.36] |
| Accept | [
text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7] |

## Headers de Response

| Header       | Valor                           | Significado |
|--------      |-------                          |-------------|
| Content-Type | application/json; charset=utf-8 | Indica que la respuesta contiene datos en formato JSON. |
| Cache-Control | [max-age=43200]                | Especifica las reglas que indican a navegadores y servidores intermedios cómo y durante cuánto tiempo pueden almacenar en caché la respuesta. |

## Comparacion

| Petición      | Content-Type                    | Contenido   |
| ------------- | ------------------              | ----------- |
| example.com   | text/html                       | Página HTML |
| /posts/1      | application/json; charset=utf-8 | Datos JSON  |


## Respuesta JSON

La respuesta contiene un objeto JSON con los campos `userId`, `id`, `title` y `body`.

## Recurso inexistente

Se realizó una petición GET a:

https://jsonplaceholder.typicode.com/posts/999

El servidor respondió con:

**404 Not Found**

Esto indica que el recurso solicitado no existe.

## Comparación HTTP vs API REST

La petición a `example.com` devuelve una página web cuyo contenido corresponde a HTML, mientras que la API REST devuelve datos estructurados en formato JSON. Por esta razón, el `Content-Type` de la página web corresponde a `text/html`, mientras que el de la API corresponde a `application/json`. Ambas solicitudes utilizan el método GET, pero tienen propósitos diferentes: la primera solicita una página web y la segunda solicita datos de un recurso de una API REST.

## Conclusión

[Completar]