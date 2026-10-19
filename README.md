# Cabezón

Juego online para jugar con amigos desde el móvil o el ordenador. Sale una categoría y cada jugador tiene que decir algo que encaje antes de pasar la cabeza. Cuanto más rara es la respuesta, más puntos da, pero también la calienta más. Si la cabeza te revienta en las manos, pierdes una vida.

## Cómo se juega

1. Uno pulsa **Crear partida** y le sale un código de 4 números.
2. Los demás abren la misma web, escriben su nombre y el código, y pulsan **Unirme**.
3. El anfitrión pulsa **Empezar**.

| Respuesta | Puntos | Efecto en la cabeza |
|-----------|--------|---------------------|
| Común     | 1      | la enfría 1 s       |
| Media     | 2      | la calienta 2 s     |
| Rara      | 3      | la calienta 4 s     |

## Publicar en GitHub Pages

En el repositorio, ve a **Settings → Pages**, elige la rama `main` y la carpeta `/ (root)`, y guarda. En un par de minutos el juego estará en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Técnica

- Es un único archivo, `index.html`, sin compilar nada.
- La conexión entre jugadores es directa entre navegadores, con [PeerJS](https://peerjs.com/).
- **Base de datos de trivial en español.** 82 categorías y más de 5.000 respuestas, organizadas con los mismos temas que Open Trivia Database: cine, música, televisión, videojuegos, ciencia, geografía, historia, mitología, deportes, arte, libros, cómics, anime, dibujos animados, tecnología, vehículos, juegos de mesa y cultura general. Cada respuesta está clasificada como común, media o rara.
- **Segunda fuente: [Wikidata](https://www.wikidata.org/).** Aproximadamente 3 de cada 10 rondas salen de aquí: películas de un director, canciones de un artista, jugadores de un club… Solo se aceptan respuestas con cierta fama, para que no salgan cosas demasiado raras.
- **Funciona sin conexión.** Si Wikidata no responde, el juego sigue solo con la base de trivial.
- El juego recuerda en el navegador qué categorías ya han salido para no repetirlas.
- El dibujo de la cabeza es original del autor.
