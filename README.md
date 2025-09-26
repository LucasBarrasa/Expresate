# Exprésate

### Cada voz cuenta.

![Demostración de la app Exprésate](https://raw.githubusercontent.com/LucasBarrasa/Expresate/874c34b8f541b5ef3dde6a40a34c941e6be93639/assets/Gift%20expresate.gif)

## 🎯 El Problema que Resuelve

Millones de personas con condiciones como discapacidad en el habla, Trastorno del Espectro Autista (TEA), afasia, ELA o secuelas de ACV enfrentan desafíos diarios para comunicarse. Las soluciones actuales suelen ser costosas, rígidas y poco adaptables al contexto personal del usuario , lo que conduce al aislamiento social y limita severamente sus oportunidades de independencia.


## ✅ La Solución Propuesta

Exprésate es una aplicación móvil nativa de Android que ofrece distintas herramientas para comunicarse, siendo la principal un sistema de comunicación intuitivo mediante pictogramas 100% personalizables. Permite a los usuarios construir y verbalizar frases de manera fluida , asegurando que la herramienta represente fielmente el mundo y las necesidades de quien la usa. El objetivo es consolidarse como un centro de accesibilidad integral que se adapte a los usuarios, mejore continuamente y vaya incluyendo nuevas herramientas como la recien agregada de texto a voz que ya se encuentra disponible y las que se vienen en camino como la de Voz a texto.


## ✨ Funcionalidades Clave

* Motor de Comunicación SAAC: Sistema de pictogramas con reproducción de voz y un constructor de frases dinámico.
* Integración Text-to-Speech (TTS): Utiliza el motor nativo de Android para una verbalización clara, fluida y 100% offline para no estar limitado a la necesidad de una coneccion a internet para su uso.
* Gestión Completa de Contenidos (CRUD): Permite crear, editar, borrar y organizar pictogramas y categorías.
* Personalización Extrema: Importación de imágenes desde la galería del dispositivo, a través del Photo Picker para nuevas APIs, y desde internet (API de ARASAAC).
* Interfaz Dinámica: Gestión de contenido con funcionalidad de arrastrar y soltar (drag-and-drop) para una fácil organización.
* Chat de texto a voz: Seccion donde personas alfabetizadas con discapacidades en el habla pueden escribir lo que desean comunicar y reproducirlo en voz alta para comunicarse con su entorno.


## 🛠️ Stack Tecnológico y Arquitectura

El proyecto fue liderado, diseñado y desarrollado implementando una arquitectura robusta y un stack tecnológico moderno para garantizar la calidad y escalabilidad del código.

* Lenguaje: Kotlin.
* Arquitectura: Se siguen los principios de Clean Architecture y el patron de presentacion MVVM.
* Interfaz de Usuario (UI): Sistema híbrido combinando XML (Views) y Jetpack Compose .
* Navegación: Jetpack Navigation Component.
* Asincronía: Coroutines y Flow para el manejo de estados de UI asíncronos.
* Persistencia de Datos: Base de datos local con Room, incluyendo data pre-cargada.
* Consumo de APIs: Retrofit y OkHttp para la gestión de llamadas a la API REST de ARASAAC.
* Inyección de Dependencias: Dagger/Hilt para asegurar un código modular, escalable y testeable.
* Librerías Adicionales: Glide y Coil para carga de imágenes, Firebase con sus herramientas como: Analitycs, Crashlytics, Auth, FireStore.
* Seguridad y optimisacion: ProGuard, R8 para la limpieza de codigo no utilizado y la seguridad ofuscando el codigo.
* Herramientas: Android Studio, Git, GitHub.


## 🗺️ Roadmap (Hoja de Ruta)

El desarrollo del proyecto se plantea de manera evolutiva y estratégica.

### En Desarrollo (Corto Plazo) 

[x] Refactorizacion de toda la app, donde se implemento la modularizacion siguiendo los lineamientos de Clean Architecture e interconectando los modulos a travez del uso de injeccion de dependencia para mejorar la escalabilidad de la app con todas las cosas nuevas que se vienen.
[x] Implementación de herramientas de texto a voz.
[x] Integracion con Room para el guardado de los mensajes escritos por el usuario.
[ ] Afinamiento de utilidad de texto a voz.
[ ] Implementación de herramientas de que ayuden a personas con discapacidad auditiva.
[ ] Creacion de loggin.
[ ] Seccion de ajustes para personalizacion y guardado de esta.

### Visión Estratégica (Futuro)

Plataforma Institucional (B2B): Desarrollo de un modelo de negocio brindar una potente plataforma de accesibilidad que permita a organizaciones mejorar sus responsabilidad social empresarial y ser mas inclusivas.
Funcionalidades Premium: Copia de seguridad en la nube , gestión de múltiples paneles para especialistas y ajustes de configuración de voz.
Innovación en Accesibilidad: Desarrollo de un módulo para el manejo de la app solo con la vista.
Expansión: Análisis de viabilidad para la expansión a otras plataformas como iOS-


## ✍️ Contacto
* LinkedIn: linkedin.com/in/lucas-barrasa-dev/ 
* GitHub: github.com/LucasBarrasa 
* Email: lucasbarrasa.dev@gmail.com 
