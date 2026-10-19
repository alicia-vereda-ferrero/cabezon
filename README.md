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
- El dibujo de la cabeza es original del autor.
