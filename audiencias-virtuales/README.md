# audiencias-virtuales 🌍⚖️

Cinco mini-juegos sueltos y autocontenidos bajo un mismo hilo narrativo: **"Tribunal de la Distancia"** — la relación está en juicio contra los kilómetros y el tiempo. Cada juego es una audiencia distinta; el veredicto siempre se gana, pero no siempre es lo mismo.

Pensado para enviarse de uno en uno, sin orden ni calendario fijo — cuando surja, en una semana o en dos meses.

## El pozo de premios

A diferencia de la primera versión (todo terminaba en "cena"), ahora cada veredicto sale al azar de un **pozo de premios mixto**, definido en el array `PREMIOS` dentro de cada archivo:

- **🌷 real** — algo físico que tú envías de verdad (delivery de flores, dulces, un regalo, una carta por correo).
- **🤝 promesa** — algo para cuando se vean, o virtual mientras tanto (videollamada-cine, una cena, playa, parque, una llamada larga, una visita prometida).

Cada resultado muestra una etiqueta (`📬 Regalo real` / `🤝 Promesa`) y un sello distinto (`ENTREGA AUTORIZADA` / `PROMESA REGISTRADA`) para que quede claro qué tipo de premio le tocó, sin que tengas que estar tú mismo explicándoselo.

## Proyectos

| Archivo | Mecánica |
|---|---|
| [`ruleta_audiencias.html`](./ruleta_audiencias.html) | Ruleta: cada segmento ES un premio del pozo, gira y decide |
| [`sello_confidencial.html`](./sello_confidencial.html) | Rasca y gana: el premio se sortea al cargar la página, oculto bajo el sello |
| [`examen_barra_amor.html`](./examen_barra_amor.html) | Trivia de pareja sobre la distancia; puntaje decorativo, premio al azar al final |
| [`reconstruye_pruebas.html`](./reconstruye_pruebas.html) | Puzzle deslizante 3×3, siempre resoluble; premio al azar al resolverlo |
| [`recurso_inapelable.html`](./recurso_inapelable.html) | Tres en raya contra una IA invencible (minimax); premio al azar sea cual sea el resultado |

## Importante: por qué el array está repetido 5 veces

A propósito, `PREMIOS` está **duplicado igual en los 5 archivos** en vez de compartido en un solo `premios.js`. Así cada juego sigue siendo un único archivo HTML autocontenido — puedes mandar cualquiera de los 5 suelto por WhatsApp como documento y funciona sin depender de los otros. El costo es que si cambias el pozo de premios, hay que copiar el cambio en los 5 archivos.

## Personalizar

- **Pozo de premios:** array `PREMIOS` en cada archivo (busca el comentario `EDITA AQUÍ`). Mantenlos realistas — son cosas que de verdad le vas a poder cumplir.
- **Preguntas de la trivia:** array `preguntas` en `examen_barra_amor.html` (las opciones vienen como placeholder, hay que rellenarlas con las reales).
- **Colores:** variables CSS `:root` al inicio de cada `<style>` (mismas variables en los 5 archivos).

## Desplegar en GitHub Pages

Si ya tienes Pages activado, quedan disponibles en:
`https://<usuario>.github.io/grachi/audiencias-virtuales/ruleta_audiencias.html` (y así con cada archivo).
