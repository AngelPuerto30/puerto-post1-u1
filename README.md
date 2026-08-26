# Post-contenido — Unidad 1: Fundamentos de la Web

## Descripción
Repositorio del laboratorio de la Unidad 1 de Programación Web —
Séptimo Semestre. Contiene dos partes: configuración del entorno
de desarrollo (parte-1-entorno/) y análisis de peticiones HTTP con
Chrome DevTools y Postman (parte-2-analisis-http/).

## Parte 1 — Entorno de desarrollo
Página HTML básica inspeccionada con Chrome DevTools. Ver
parte-1-entorno/.

## Parte 2 — Análisis de peticiones HTTP
| # | Tipo | URL | Código |
|---|------|-----|--------|
| 1 | GET HTML | https://example.com | 200 OK |
| 2 | GET JSON (exitoso) | /posts/1 | 200 OK |
| 3 | GET JSON (fallido) | /posts/999 | 404 Not Found |
| 4 | POST JSON | /posts | 201 Created |

Ver parte-2-analisis-http/analisis/.

## Herramientas utilizadas
- VS Code, Git, GitHub
- Google Chrome + DevTools (panel Network)
- Postman (petición POST con tests)

## Conclusiones
El laboratorio permitió reforzar los conocimientos sobre la estructura básica de una página web y el uso de herramientas de desarrollo mediante VS Code, Git y Chrome DevTools. En la segunda parte se analizaron peticiones HTTP utilizando los métodos GET y POST, identificando códigos de estado como 200, 201 y 404, además de diferencias entre respuestas HTML y JSON. También se comprendió la importancia de los headers HTTP, los tiempos de carga y el funcionamiento de las solicitudes y respuestas entre cliente y servidor. Finalmente, el uso de Postman permitió realizar peticiones POST y validar automáticamente sus resultados mediante tests, fortaleciendo la comprensión práctica del funcionamiento de las API REST.
