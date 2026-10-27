# 🐉 Spyro The Dragon — Android Guide & Explorer

![Android](https://img.shields.io/badge/Android-Java-3DDC84?style=for-the-badge&logo=android)
![Arquitectura](https://img.shields.io/badge/Arquitectura-Fragments_%26_Navigation-informational?style=for-the-badge)
![UI](https://img.shields.io/badge/Material_Design-CardView-blue?style=for-the-badge&logo=google)
![IDE](https://img.shields.io/badge/Android_Studio-Ladybug%20%7C%20Koala-4285F4?style=for-the-badge&logo=androidstudio)

Una aplicación móvil nativa desarrollada en **Java para Android** inspirada en el universo del clásico videojuego **Spyro the Dragon**. El proyecto implementa una arquitectura modular basada en componentes de navegación modernos de Jetpack, adaptadores dinámicos para listas complejas y soporte de temas personalizados.

---

## 📱 Características Principales

- **🧭 Navegación Fluida:** Implementación de `BottomNavigationView` integrada con el componente **Jetpack Navigation Graph** (`nav_graph.xml`) para transiciones limpias y gestión eficiente de la pila de fragmentos.
- **🏰 Sección de Mundos:** Exploración de los reinos del juego mediante un `RecyclerView` personalizado que muestra imágenes, descripción y características de cada mundo en `CardView`.
- **💎 Coleccionables y Joyas:** Catálogo interactivo de gemas, huevos de dragón y estatuas con información y conteo.
- **🐲 Personajes y Guía Interactiva:** Vista detallada de personajes con bocadillos de diálogo personalizados (`bocadillo_personajes.xml`) estilo cómic/retro.
- **🌓 Soporte Modo Noche / Día:** Adaptación completa a temas claros y oscuros respetando las directrices de Material Design.
- **📄 Extracción de Datos:** Desacoplamiento de la lógica mediante recursos XML estructurados (`res/raw/characters.xml` y `worlds.xml`) parseados en tiempo de ejecución.

---

## 🏗️ Arquitectura y Estructura del Código

El proyecto sigue una organización limpia por capas:

```text
dam.pmdm.spyrothedragon/
│
├── 📂 adapters/          # Adaptadores de RecyclerView optimizados
│   ├── CharactersAdapter.java
│   ├── CollectiblesAdapter.java
│   └── WorldsAdapter.java
│
├── 📂 models/            # Modelos de dominio
│   ├── Character.java
│   ├── Collectible.java
│   └── World.java
│
├── 📂 ui/                # Fragmentos de la interfaz de usuario
│   ├── CharactersFragment.java
│   ├── CollectiblesFragment.java
│   └── WorldsFragment.java
│
├── MainActivity.java     # Host de navegación y barra inferior
└── WelcomeActivity.java  # Pantalla de bienvenida / onboarding
```

---

## 🛠️ Tecnologías y Componentes Utilizados

- **Lenguaje:** Java 11 / 17.
- **Android SDK:** Min SDK 24 / Target SDK 34+.
- **Android Jetpack:**
  - Navigation Component (`NavController`, `NavHostFragment`).
  - RecyclerView & CardView.
- **Diseño de Interfaz:** ConstraintLayout, Drawables vectoriales personalizados (`.xml`), Material Components.

---

## 🚀 Cómo Ejecutar el Proyecto

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/BLL75/SpyroTheDragon.git
   ```

2. **Abrir en Android Studio:**
   - Selecciona `File` > `Open` y elige la carpeta del proyecto.
   - Deja que **Gradle** sincronice las dependencias del proyecto.

3. **Ejecutar en Emulador o Dispositivo Físico:**
   - Presiona `Shift + F10` o el botón verde **Run**.

---

## 👨‍💻 Autor

- **Bernardo Luque** — [GitHub @BLL75](https://github.com/BLL75)
- Proyecto desarrollado para el módulo de **Programación Multimedia y Dispositivos Móviles (DAM)**.
