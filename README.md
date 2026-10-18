# Mascaradas: El Legado

**Sigue la ronda de las mascaradas de invierno de Zamora antes de que El Olvido las apague.**

Juego de plataformas y acción en 2D sobre las mascaradas de invierno de la provincia de Zamora, escrito en HTML y Canvas puro, en un solo archivo y sin dependencias.

![Pantalla de título](prensa/capturas/00-titulo.png)

## Jugar

- **En el navegador:** <https://albertoabascal13-lgtm.github.io/mascaradas-el-legado/>
- **En itch.io:** pendiente de publicar
- **En local:** descarga `index.html` y ábrelo con doble clic. No necesita servidor ni conexión a internet.

## De qué va

De San Esteban a Carnaval, en los pueblos de Zamora salen las máscaras: diablos, zangarrones, carochos, visparras, tafarrones. Recorren las calles, piden el aguinaldo y espantan lo malo del año. Pero este invierno los cencerros suenan menos: hay pueblos donde nadie se acuerda de sacar la careta. Los viejos lo llaman por su nombre: **El Olvido**.

Eres un mozo de Aliste en su primer año de máscara. Ponte la careta, cuélgate los cencerros, coge las tenazas y sigue la ronda por trece rincones de la provincia hasta la plaza de la catedral.

## La ronda

| # | Nivel | Jefe |
|---|---|---|
| 1 | Aliste | La Helada |
| 2 | El robledal | La Sombra |
| 3 | Sierra de la Culebra | El Lobo de la Culebra |
| 4 | Sanabria | La Campana de Lucerna |
| 5 | Tábara | La Cabeza Parlante |
| 6 | Pozuelo | El Ramo |
| 7 | El Scriptorium | La Bestia del Beato |
| 8 | Sayago | El Berrueco |
| 9 | Almeida | El Verraco |
| 10 | La plaza | El Diablo Mayor |
| 11 | El Cerro de la Ermita | La Falsa Madama |
| 12 | Las Aceñas | El Barquero |
| 13 | La Ciudad | El Olvido |

## Qué trae

- **13 niveles** inspirados en lugares reales: Aliste, la Sierra de la Culebra, el lago de Sanabria, la torre del Beato de Tábara, el berrocal de Sayago, Almeida de Sayago, Montamarta, las aceñas del Duero y la plaza de la catedral de Zamora.
- **27 personajes** con diálogo, voz y retrato propios, casi todos mascaradas reales: los Carochos, la Filandorra, las visparras y talanqueiras, el Birria, el Tafarrón y la Madama, la Vaca Bayona, el Zangarrón.
- **13 jefes** sacados de leyendas y paisajes de la provincia, y **18 tipos de enemigo**, cada nivel con uno propio.
- **Un diario de 17 fichas** con la historia real de cada tradición, que se va abriendo mientras juegas, y una pantalla de **fuentes** con los trabajos y reportajes en que se basa cada una.
- Combate con tres armas (tenazas, palo de vejigas y alforja de ceniza), agacharse, rodada con invulnerabilidad y golpes arriba, abajo y a ras de suelo.
- Secuenciador de audio propio: dulzaina, bordón y tamboril, con un tema por comarca y variaciones para que el bucle no canse.
- **Tres rondas de dificultad** con nombres del folklore: Filandón, Obisparra y Antruejo.
- **Modo ronda completa**: los 13 niveles seguidos con tres vidas y marcador de aguinaldo.
- Dos estilos gráficos, guardado automático en cada hoguera y marcador de récords.
- Teclado, mando y botones táctiles; teclas reasignables, tamaño de botones y opciones de temblor y parpadeos.

## Controles

| | Teclado | Mando | Móvil |
|---|---|---|---|
| Moverse | ← → | Stick o cruceta | ◀ ▶ |
| Saltar | Espacio | A | ⤒ |
| Golpear / usar | J | X | ✠ |
| Agacharse | ↓ | Abajo | ▼ |
| Rodar | K | RB / LB | ⟳ |
| Cambiar arma | L | Y | ⇄ |
| Pausa | P | Start | ⏸ |
| Música | M | Select | 🔔 |

Todas las teclas se pueden cambiar en **Ajustes → Teclas**. Con mando, pulsa cualquier botón una vez al empezar para que el navegador lo detecte.

Golpea junto a los personajes, los letreros y las hogueras para usarlos. Las hogueras curan y guardan la partida.

## Cómo está hecho

Un único `index.html` de unos 340 KB con todo dentro: motor, sprites, textos, música y las dos tipografías incrustadas. No usa librerías, ni compilación, ni peticiones de red.

- **Gráficos:** Canvas 2D a 320×180 escalado con pixelado nítido. Los sprites son arrays de cadenas con una paleta por personaje, y cada nivel tiene una paleta alternativa para el segundo estilo gráfico.
- **Sonido:** Web Audio API. Osciladores, filtros y búferes de ruido generados en el momento; no hay ni un archivo de audio. La música baja de volumen durante los diálogos.
- **Guardado:** `localStorage`, con partida, récords, ajustes y teclas.
- **Mando:** Gamepad API, con disposición estándar y navegación de los menús.

Para tocarlo basta con abrir el archivo en un editor; todo el código está en el bloque `<script>` del final.

## Capturas

En [`prensa/capturas`](prensa/capturas) están los trece niveles, la pantalla de título, el recuento de fin de nivel y la botonera táctil. La portada para tiendas está en [`prensa/portada-630x500.png`](prensa/portada-630x500.png).

## Créditos y fuentes

Idea, historia y dirección: **alberto_hdez13**. Desarrollado con ayuda de Claude (Anthropic).

Juego de ficción: personajes, escenarios y leyendas están adaptados con libertad. Dentro del juego, en **Fuentes**, se citan los dieciséis bloques de documentación real en que se basa cada mascarada, con los trabajos y reportajes consultados.

Las tipografías incrustadas son [Pirata One](https://fonts.google.com/specimen/Pirata+One) y [Spectral](https://fonts.google.com/specimen/Spectral), ambas bajo SIL Open Font License 1.1.

## Licencia

Por decidir. Hasta que se añada un archivo `LICENSE`, todos los derechos quedan reservados al autor.
