Sesión 1 — Empatizar + Configuración inicial (ODS y usuarios)

Juan de la Vega 
Emiliano Ramírez A00574759
Fabricio Padilla
Enrique Camarena A00574884
Patricio Hinojosa A00575222

👩‍💼 Product Owner (PO) JUAN DÍAZ DE LA VEGA
Es la persona que mantiene la visión del proyecto. Se asegura de que el prototipo responda al ODS seleccionado y a las necesidades de la población objetivo. Prioriza las funcionalidades, organiza el trabajo en el tablero Kanban y lidera la presentación tipo Shark Tank.

👨‍💻 Líder Técnico (Tech Lead) ENRIQUE CAMARENA 
Se encarga de la arquitectura y calidad del código. Define cómo se organizan los módulos del proyecto, revisa que el código cumpla con estándares y apoya al equipo en resolver problemas técnicos complejos. Su responsabilidad es que el prototipo funcione de manera estable.

🖥️ Desarrollador UI (Interfaz de Usuario) FABRICIO PADILLA
Diseña y programa las pantallas y la experiencia de usuario con PySimpleGUI. Se asegura de que la app sea clara, fácil de usar y que los botones, entradas y mensajes funcionen correctamente. Traduce la lógica técnica a una interacción amigable para el usuario.

📊 Desarrollador de Datos/API EMILIANO RAMÍREZ MENDOZA 
Implementa el manejo de datos y la conexión con fuentes externas. Trabaja con pandas para leer y procesar archivos, integra al menos una API pública y prepara los datos para ser usados en el prototipo. Su tarea es garantizar que la aplicación tenga información real y confiable.

🧪 QA / Analista de Pruebas PATRICIO HINOJOSA
Se encarga de la calidad del software. Diseña y ejecuta pruebas de caja negra, identifica errores y verifica que los criterios de éxito definidos se cumplan. También documenta resultados y prepara evidencias para mostrar la solidez del prototipo.


2. Selección de ODS y población objetivo
ODS elegido: ODS 14 – Vida submarina
“Conservar y utilizar sosteniblemente los océanos, los mares y los recursos marinos para el desarrollo sostenible.”

Problemática detectada
Contaminación por plásticos y basura marina: millones de toneladas de plásticos y microplásticos llegan cada año a los océanos, afectando a peces, tortugas, aves marinas y ecosistemas enteros.
Sobrepesca: muchas especies marinas están siendo explotadas a tasas insostenibles, poniendo en riesgo la seguridad alimentaria y la biodiversidad.
Degradación de arrecifes y hábitats marinos: la contaminación, el cambio climático y la pesca con métodos destructivos dañan hábitats vitales como manglares, corales y pastos marinos.

Población objetivo
Jóvenes universitarios: para fomentar conciencia ambiental y proyectos de innovación en reciclaje, reducción de plásticos y tecnologías de monitoreo.
Comunidades costeras y pesqueras: directamente afectadas por la sobrepesca y la contaminación.
Ciudadanía en general: porque el consumo de plásticos y de productos del mar impacta directamente en la sostenibilidad de los océanos.

Evidencias (datos, ejemplos, noticias)
Contaminación plástica en océanos
Cada año se generan más de 460 millones de toneladas de plástico, de las cuales al menos 14 millones terminan en los océanos.
Se estima que el 85% de la basura marina es plástico (botellas, bolsas, redes de pesca, microplásticos).
(Fuente: Programa de las Naciones Unidas para el Medio Ambiente – PNUMA, 2022)
Impacto en biodiversidad marina
Más de 700 especies marinas han sido afectadas por plásticos en el mar (ingestión, enredo, pérdida de hábitat).
Estudios muestran que el 90% de las aves marinas tienen plástico en su sistema digestivo y que los microplásticos ya se detectan en peces y mariscos consumidos por humanos.
(Fuente: IUCN – International Union for Conservation of Nature, 2023)

Detección de basura marina (IA)
Entrenar un modelo de Machine Learning / Deep Learning que clasifique imágenes submarinas (ej. detectar plásticos, redes o peces).
Librerías: TensorFlow, PyTorch, OpenCV.
Dataset: “Marine Debris Dataset” de Kaggle.
Podría servir a ONGs o proyectos ciudadanos para monitorear playas.
 Sistema de monitoreo comunitario
Una app donde pescadores/turistas suben datos:
Si vieron plásticos.
Avistamiento de especies.
Calidad del agua (si tienen sensor barato).
La app genera un mapa colaborativo en tiempo real.
Backend en Python (Flask/Django) + base de datos + frontend simple.






















