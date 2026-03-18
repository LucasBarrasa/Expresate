## Exprésate: Sistema de Comunicación Alternativa y Aumentativa (SAAC)

Exprésate es una aplicación nativa de Android diseñada para resolver barreras de comunicación complejas. Actúa como una herramienta integral offline-first, ofreciendo un sistema dinámico de pictogramas y un módulo de chat TTS/STT (Texto a Voz / Voz a Texto).

![Demostración de la app Exprésate](https://raw.githubusercontent.com/LucasBarrasa/Expresate/874c34b8f541b5ef3dde6a40a34c941e6be93639/assets/Gift%20expresate.gif)

## 🚀 Impacto y Validación en el Mundo Real
A diferencia de proyectos teóricos, Exprésate está validado en entornos de producción críticos:

* Implementación Institucional: Adoptado oficialmente por el área de Discapacidad del Municipio de Dolores (Buenos Aires).
* Participacion en InnovELA: Se participo con la App en la primera edición de la exposición InnovELA, realizada por la fundación Esteban Bullrich.
* Expansión B2B/B2G: Actualmente en fase de escalado para su integración en centros de salud municipales y áreas de atención al público general, facilitando la inclusión en comercios e instituciones.


## ✨ Funcionalidades Clave

* Motor de Comunicación SAAC: Sistema de pictogramas con reproducción de voz y un constructor de frases dinámico.
* Integración Text-to-Speech (TTS): Utiliza el motor nativo de Android para una verbalización clara, fluida y 100% offline para no estar limitado a la necesidad de una coneccion a internet para su uso.
* Gestión Completa de Contenidos (CRUD): Permite crear, editar, borrar y organizar pictogramas y categorías.
* Personalización Extrema: Importación de imágenes desde la galería del dispositivo, a través del Photo Picker para nuevas APIs, y desde internet (API de ARASAAC).
* Interfaz Dinámica: Gestión de contenido con funcionalidad de arrastrar y soltar (drag-and-drop) para una fácil organización.
* Chat de texto a voz: Seccion donde personas alfabetizadas con discapacidades en el habla pueden escribir lo que desean comunicar y reproducirlo en voz alta para comunicarse con su entorno.


## 🏗️ Arquitectura y Stack Tecnológico

El proyecto está diseñado bajo los principios de Clean Architecture (Dominio, Datos, Presentación), permitiendo alta escalabilidad y testeabilidad. Actualmente se encuentra en un proceso de modularización y migración progresiva hacia UI declarativa.

* Lenguaje: Kotlin (100%).
* Arquitectura: Se siguen los principios de Clean Architecture y el patron de presentacion MVVM.
* UI / Presentación: Enfoque híbrido. Migración activa de XML/Views hacia Jetpack Compose. Gestión de estado reactivo mediante StateFlow y eventos únicos a través de Channels.
* Inyección de Dependencias: Dagger/Hilt para acoplamiento débil entre capas.
* Asincronismo y Concurrencia: Kotlin Coroutines & Flow.
* Persistencia (Offline-First): Base de datos local robusta utilizando Room para garantizar la disponibilidad del sistema sin conexión a internet (crítico para usuarios en cualquier contexto).
* Red: Retrofit y OkHttp para sincronización bajo demanda con la API de ARASAAC (descarga de pictogramas).
* Infraestructura: Firebase Crashlytics & Analytics para monitoreo de estabilidad.
* Navegación: Jetpack Navigation Component.
* Librerías Adicionales: Glide y Coil para carga de imágenes
* Seguridad y optimisacion: ProGuard, R8 para la limpieza de codigo no utilizado y la seguridad ofuscando el codigo.
* Herramientas: Android Studio, Git, GitHub.


## ⚙️ Características Técnicas Destacadas

* Gestión de Estado Complejo: El asistente de pictogramas y el módulo STT/TTS manejan múltiples estados asíncronos en tiempo real, controlando el ciclo de vida de los motores nativos de procesamiento de lenguaje de Google.

* Estrategia Caching / Offline: Los pictogramas descargados desde ARASAAC se indexan en Room y se almacenan localmente en el dispositivo, asegurando latencia cero y funcionamiento en zonas sin cobertura.

* Modularización: El nuevo feature de Chat Bidireccional (STT/TTS) fue desarrollado como un módulo independiente, marcando el inicio de la fragmentación del monolito para mejorar tiempos de compilación y separación de responsabilidades.


## 🗺️ Próximos Pasos (Roadmap Técnico)

* Finalizar migración total a Jetpack Compose.
* Deprecación de LiveData en módulos antiguos en favor de Kotlin Flow.
* Implementación de CI/CD con GitHub Actions para automatizar el testing y despliegue a Play Store.
* Sostenibilidad: Desarrollo de un modelo de negocio evolutivo y sostenible para un crecimiento de la plataforma y que les permita a organizaciones mejorar sus responsabilidad social empresarial y ser mas inclusivas.  
* Expansión: Análisis de viabilidad para la expansión a otras plataformas como iOS.  



## ✍️ Contacto
* LinkedIn: linkedin.com/in/lucas-barrasa-dev/ 
* GitHub: github.com/LucasBarrasa 
* Email: lucasbarrasa.dev@gmail.com  
