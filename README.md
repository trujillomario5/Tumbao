# Tumbao

Generador de canciones en español, de código abierto (licencia MIT).

Escribe o genera una letra, elige un género y escúchala cantada al momento. Todo funciona en el navegador: sin servidor, sin cuentas y sin claves de API.

## Cómo usarlo

1. Abre `index.html` en Chrome, Edge, Firefox o Safari (doble clic basta).
2. Elige un tema (Fiesta, Amor, Desamor, Mi tierra, Superación, Cumpleaños), escribe una idea o título y, si quieres, a quién va dedicada.
3. Pulsa **Escribir letra** u **Otra versión**, o pega tu propia letra. Marca las partes con `[Verso]`, `[Coro]`, `[Puente]`, `[Intro]`.
4. Elige el género y la voz, y pulsa ▶.
5. **Descargar WAV** guarda la canción completa (solo aparece al abrir el archivo directamente, no dentro de un visor incrustado).

## Géneros incluidos (21)

Salsa, son cubano, vallenato, cumbia, bachata, merengue, reggaetón, dembow, trap latino, pop latino, rock en español, balada, bolero, ranchera (3/4), corrido tumbado, afrobeat, champeta, tango, rumba flamenca, bossa nova y reggae.

Cada género define su tempo, tonalidad, progresión de acordes, instrumentos y patrones rítmicos (por ejemplo, la clave 2-3 en salsa y son, el dembow 3-3-2 en reggaetón, la guacharaca en vallenato y cumbia, la cadencia andaluza en rumba). Para añadir uno nuevo, agrega un objeto al arreglo `GENRES` en el código.

## Cómo funciona

- **Música:** síntesis en vivo con Web Audio API (tambores, congas, bongó, tambora, güiro, guacharaca, güira, bajo, 808, piano, acordeón, metales, guitarras, órgano). No usa muestras grabadas.
- **Cantante sintético:** separa la letra en sílabas (con reglas del español y sinalefa), genera una melodía sobre los acordes del género y canta cada vocal con un sintetizador de formantes. Suena a voz robótica, no a un cantante real.
- **Voz narrada:** usa la voz en español del navegador (Web Speech API).
- **Letras:** generador local con versos rimados por tema; no necesita internet.

## Voz realista con IA abierta (opcional)

El botón **Copiar letra y estilo** prepara el texto con etiquetas (`[verse]`, `[chorus]`, `[bridge]`) y una descripción del estilo del género. Puedes pegarlo en modelos abiertos de generación de canciones que cantan en español, por ejemplo:

- **ACE-Step** (Apache 2.0): https://github.com/ace-step/ACE-Step
- **YuE** (Apache 2.0): https://github.com/multimodal-art-projection/YuE

Ambos se ejecutan en tu propio equipo y funcionan mejor con una GPU NVIDIA. No necesitan claves de pago.

## Licencia

MIT. Úsalo, cámbialo y compártelo libremente.
