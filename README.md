# LA-ELITE
un asistente el cual me ayude a predecir los mejores resultados para apuestas deportivas
 ## 1. Perfil del Agente.
<img width="1336" height="748" alt="Mapa Mental Curvado hacia abajo" src="https://github.com/user-attachments/assets/2ec31730-c9a0-456c-8a36-e447b66eb381" />
## 2. Mapa de procesos.
<img width="781" height="719" alt="Captura de pantalla 2026-08-21 114637" src="https://github.com/user-attachments/assets/61da5d29-40b9-493b-b8b3-efcdd7d25303" />
justificacion teorica breve: Mi bot necesita mucha memoria (10/10) porque debe procesar y memorizar muchos datos deportivos para que el cliente pueda tener una apuesta sobresaliente y exitosa, tambien necesita bastante pensamiento y razonamiento (9/10) porque necesita pensar, analizar y razonar todos los datos que recopila en su memoria segun el evento deportivo los eventos deportivos que el usuario quiera apostarle, tambien aunque necesita menos lenguaje (7/10) debe poder expresarse aunque sencillo, debe expresarse de forma profesional y en los distintos idiomas que se le pueda ofrecer al cliente, necesita menos atencion (5/10) si, pero no es que sea totalmente innecesaria ya que debe poder tener una buena atencion para con el usuario y lo que el desea y por ultimo aunque es la mas poca que seria la emocion (4/10) por que considero que noes tan necesario ya que mi bot va a lo que va y ya que tiene un perfil mas profesional no necesita tanto las emociones.
## 3. Diagrama de Flujo y Inputs
<img width="1160" height="729" alt="Captura de pantalla 2026-08-28 121222" src="https://github.com/user-attachments/assets/ce618f51-7ef1-474c-8d07-c98a8763c54a" />
<img width="1291" height="738" alt="Captura de pantalla 2026-08-28 124247" src="https://github.com/user-attachments/assets/6c0dbc6a-44ed-480f-94c9-597a05f9785f" />
## 4. Arquitectura de atencion con las reglas logicas definidas
Reglas de Atención. Identificación de la intención: primero identificará qué evento deportivo y qué información solicita el usuario, Priorización de datos relevantes: dará mayor atención a los datos directamente relacionados con el evento, como equipos o jugadores, estadísticas, resultados recientes y demás información necesaria para el análisis, Filtrado del ruido: ignorará información que no tenga relación directa con la predicción solicitada, Mensajes extensos: si el mensaje tiene más de 500 palabras, el mecanismo de atención priorizará los sustantivos clave, los datos deportivos relevantes y la última frase, con el objetivo de reducir la carga cognitiva del sistema, Información contradictoria: cuando encuentre datos que se contradigan, los marcará para que el mecanismo de razonamiento pueda analizarlos antes de utilizarlos, Prioridad al objetivo del usuario: la información relacionada directamente con la apuesta o evento solicitado tendrá mayor prioridad que la información secundaria, Conservación de información importante: los datos considerados relevantes serán enviados a la memoria y al módulo de razonamiento para continuar con el análisis.
## 5. Esquema de la Base de Conocimiento
| Tipo de memoria     | Categoría / carpeta           | Información que almacenará                                         | Ejemplos                                                 |
| ------------------- | ----------------------------- | ------------------------------------------------------------------ | -------------------------------------------------------- |
| **LTM – Semántica** | Deportes                      | Conocimientos generales sobre los diferentes deportes              | Fútbol, baloncesto, tenis, béisbol                       |
| **LTM – Semántica** | Equipos y jugadores           | Información general y características de equipos y jugadores       | Plantillas, posiciones, ligas, historial general         |
| **LTM – Semántica** | Estadísticas deportivas       | Conceptos y tipos de estadísticas utilizados para analizar eventos | Promedio de goles, puntos, victorias, derrotas           |
| **LTM – Semántica** | Competiciones                 | Conocimiento sobre ligas y torneos                                 | Champions League, Liga BetPlay, NBA, ATP                 |
| **LTM – Semántica** | Mercados de apuestas          | Definiciones de los diferentes mercados que puede analizar         | Ganador, hándicap, goles, puntos, ambos marcan           |
| **LTM – Semántica** | Factores de análisis          | Conocimientos sobre factores que pueden influir en un evento       | Localía, rendimiento, lesiones, descanso, clima          |
| **LTM – Largo plazo** | Eventos deportivos            | Registro de eventos deportivos específicos                         | Partido, fecha, equipos participantes y resultado        |
| **LTM – Episódica** | Análisis realizados           | Registro de análisis realizados por LA-ELITE                       | Evento analizado, datos utilizados y análisis generado   |
| **LTM – Episódica** | Resultados de análisis        | Comparación entre análisis realizados y resultados reales          | Predicción realizada, resultado del partido y diferencia |
| **LTM – Largo plazo** | Historial de enfrentamientos  | Registro de enfrentamientos específicos entre equipos o jugadores  | Resultados de partidos anteriores entre dos equipos      |
| **LTM – Episódica** | Cuotas y mercados consultados | Registro de cuotas y mercados observados en eventos anteriores     | Mercado consultado, cuota y fecha                        |
| **LTM – Episódica** | Interacciones con usuarios    | Información relevante de las consultas realizadas por los usuarios | Evento solicitado, mercado consultado y preferencias     |
| **LTM – Episódica** | Fuentes consultadas           | Registro de las fuentes utilizadas durante cada análisis           | Fuente, fecha de consulta y datos obtenidos              |



