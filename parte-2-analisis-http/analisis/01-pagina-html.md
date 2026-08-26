# Análisis 1: Petición GET — example.com

## Información general
- URL: https://example.com/
- Método: GET
- Código de estado: [304 Not Modified]

## Headers de Request
| Header | Valor |
|--------|-------|
| Host | [example.com] |
| User-Agent | [Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/151.0.0.0 Safari/537.36] |
| Accept | [text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7] |

## Headers de Response
| Header | Valor | Significado |
|--------|-------|-------------|
| Content-Type | [No aparece] | [Indica el tipo de contenido que devuelve el servidor, por ejemplo text/html para una página HTML.] |
| Cache-Control | [No aparece] | [Especifica las reglas que indican a navegadores y servidores intermedios cómo y durante cuánto tiempo pueden almacenar en caché la respuesta.] |

## Tiempos de carga
| Fase | Tiempo (ms) |
|------|------------|
| DNS Lookup | [130.06 ms] |
| TTFB | [110.55 ms] |

## Conclusión
[La petición realizada a example.com utilizó el método GET y obtuvo un código de estado 304 Not Modified. Los headers de la petición muestran información sobre el navegador y los tipos de contenido que acepta. El DNS Lookup tardó 130.06 ms, mientras que el TTFB fue de 110.55 ms. En general, el análisis permitió observar el proceso de comunicación entre el navegador y el servidor, así como el uso de la caché para evitar descargar nuevamente un recurso que no ha cambiado.]