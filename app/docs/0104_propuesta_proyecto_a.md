# Plantilla: propuesta del Proyecto A

---

## 0 · Datos

| | |
|---|---|
| **Nombre de la app** | MelodyCatch |
| **Autor/a** | José Cerero |
| **Fecha** |   01/10/2026 |

---

## 1 · La idea en una frase

> Qué hace tu app y para quién, en una sola frase.

> Captura una melodía y hazla realidad.
> Fórmula: «Una app que permite a [quién] hacer [qué] para [para qué].»

- MelodyCatch permite capturar una idea melódica y desarrollarla hasta convertirla en una canción.



---

## 2 · El problema

> ¿Qué problema resuelve? ¿Cómo se resuelve hoy sin tu app?

- Una idea musical puede aparecer en cualquier momento, por ejemplo mientras estás caminando, y muchas veces se pierde o termina simplemente en una grabación de voz. El problema es que, después de grabarla, hay que recurrir a diferentes herramientas para descubrir su tonalidad, buscar una armonía, escribir la letra y darle una estructura. MelodyCatch busca agilizar este proceso ofreciendo desde el primer momento un entorno en el que el usuario pueda capturar la melodía y comenzar a desarrollarla directamente, convirtiendo una idea espontánea en una canción de forma más rápida y organizada.

---

## 3 · Personas usuarias

> ¿Quién la va a usar? Describe a una persona concreta: edad, soltura con la
> tecnología, cuándo y dónde abre la app, cuánto tiempo le dedica y qué pasa
> si le falla.

- La aplicación está dirigida a cualquier persona con una soltura tecnológica media y unos conocimientos básicos de música y armonía, sin necesidad de ser músico profesional.

Puede ser alguien que esté aprendiendo a tocar un instrumento, componiendo sus primeras canciones o simplemente tenga ideas melódicas y quiera desarrollarlas. Por ejemplo, mientras camina, viaja o realiza cualquier actividad cotidiana, puede surgirle una melodía y utilizar MelodyCatch para capturarla y empezar a trabajar sobre ella en ese mismo momento.

El usuario dedicaría aproximadamente entre 5 y 15 minutos a cada idea, pudiendo guardarla para continuar desarrollándola más adelante. Si la aplicación falla, podría perder una idea musical difícil de recordar, por lo que debe permitir guardar el progreso y recuperar las canciones posteriormente.

---

## 4 · Funcionalidades

### Imprescindibles (sin esto la app no tiene sentido)

| #  | Funcionalidad                                                                                      |
| -- | -------------------------------------------------------------------------------------------------- |
| F1 | Capturar y guardar una melodía                                                                     |
| F2 | Analizar la melodía y proponer una tonalidad principal y posibles tonalidades o modos relacionados |
| F3 | Añadir y editar acordes, incluyendo acordes propios y prestados de otras tonalidades o modos       |





### Opcionales (si sobra tiempo)

| #  | Funcionalidad                                        |
| -- | ---------------------------------------------------- |
| O1 | Añadir letra y organizar la estructura de la canción |
| O2 | Reproducir la melodía junto con la armonía creada    |


---

## 5 · Pantallas

| Pantalla             | Para qué sirve                                                                                                | Se llega desde   |
| -------------------- | ------------------------------------------------------------------------------------------------------------- | ---------------- |
| Mis canciones    | Muestra las melodías guardadas y permite crear una nueva.                                                         | (arranque)       |
| Capturar melodía | Permite grabar una melodía cantada o tocada con un instrumento y guardarla.                                       | Mis canciones    |
| Analizar melodía | Analiza la melodía y muestra la tonalidad principal y posibles tonalidades o modos relacionados.                  | Capturar melodía |
| Crear armonía    | Permite añadir y editar acordes, incluyendo acordes propios y acordes prestados de otras tonalidades o modos.     | Analizar melodía |


---

## 6 · Bocetos

> Dibuja las pantallas principales. A mano y fotografiado es válido.
> Pega aquí las imágenes o indica el nombre de los archivos adjuntos.

    bocetoDamProg.pdf

---

## 7 · Qué datos guarda la app

| Tipo de dato     | Campos                                                           | Ejemplo                             |
| -----------------| ---------------------------------------------------------------- | ----------------------------------- |
| Canción          | id, título, fecha de creación                                    | 1, "Mi canción", 02/10/2026         |
| Melodía          | id, canción, archivo de audio, duración                          | 1, 1, "melodia_01.wav", 12 s        |
| Análisis musical | id, canción, tonalidad principal, tonalidades/modos relacionados | 1, 1, E mayor, E menor / E dórico   |
| Armonía          | id, canción, tonalidad, progresión de acordes                    | 1, 1, E mayor, E - B - C#m - A - Am |


---

## 8 · Encaje con los requisitos del módulo

> Apartado obligatorio: ninguna casilla puede quedar vacía.

| Requisito                                                             | Dónde encaja en tu app                                                                                                    | Tema |
| --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ---- |
| **Persistencia de datos** — la información sobrevive al cerrar la app | Las canciones, melodías, acordes, letras y estructuras se guardan para poder continuar trabajando posteriormente.         | 4    |
| **Servicio web** — la app consulta datos por internet                 | La aplicación consulta una API musical para obtener información sobre escalas, notas y acordes de la tonalidad detectada. | 5    |
| **Sensor o localización**                                             | El micrófono del dispositivo se utiliza para capturar la melodía cantada o tocada por el usuario.                         | 6    |
| **Contenido multimedia** — foto, audio, vídeo o animación             | La aplicación graba, reproduce y almacena audio correspondiente a las melodías capturadas.                                | 7    |

---

## 9 · Riesgos

| Lo que me preocupa                                                                     | Plan B                                                                                              |
| -------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| El análisis automático puede no detectar correctamente la tonalidad de la melodía.     | Permitir que el usuario seleccione manualmente la tonalidad entre las propuestas.                   |
| La detección de acordes prestados puede ser demasiado compleja.                        | Permitir añadir los acordes prestados manualmente a partir de una lista de opciones.                |
| La grabación y el procesamiento de audio pueden resultar más complejos de lo previsto. | Permitir importar un archivo de audio ya grabado o trabajar inicialmente con grabaciones sencillas. |

---

## Antes de entregar

- [ ] La idea cabe en una frase.
- [ ] El público es una persona concreta, no «todo el mundo».
- [ ] Hay **3 o 4** funcionalidades imprescindibles, no diez.
- [ ] Cada funcionalidad imprescindible tiene su pantalla.
- [ ] Hay bocetos de las pantallas principales.
- [ ] **Las cuatro casillas del apartado 8 están rellenas.**
- [ ] Está identificado al menos un riesgo con su plan B.

