# XPatcher v 1.0

<img width="500" height="273" alt="logo" src="https://github.com/user-attachments/assets/20badba4-6b93-44df-aa63-6b9459a14e74" />

## Descripción

**XPatcher v 1.0r** es una herramienta de vanguardia diseñada para desarrolladores y empresas que requieren un método eficiente y seguro para distribuir actualizaciones binarias. Esta aplicación permite comparar dos versiones de un mismo ejecutable (Original y Modificado), identificar las diferencias a nivel de byte (Offsets y Valores Hexadecimales) y generar automáticamente un parcheador autónomo en C++.

El parcheador generado es un ejecutable ligero y sin dependencias que aplica los cambios directamente al archivo objetivo, ideal para procesos de actualización rápidos o correcciones "in-place" sin necesidad de reinstalaciones completas.

## Características Principales

*   **Comparación Binaria Precisa:** Analiza byte por byte para detectar cambios exactos entre versiones.
*   **Visualización Hexadecimal:** Muestra los offsets y valores antiguos/nuevos en un formato claro y técnico.
*   **Generación de Código C++:** Crea automáticamente el código fuente del parcheador, permitiendo auditorías de seguridad.
*   **Compilación Automática:** Utiliza MinGW para compilar el parcheador final en un `.exe` listo para distribuir.
*   **Interfaz Moderna (UI):** Diseño oscuro estilo "Cyberpunk/Dev" con transiciones suaves y botones circulares personalizados.
*   **Splash Screen:** Pantalla de inicio profesional con carga de imagen integrada.
*   **Ejecutable Autocontenido:** La aplicación puede compilarse en un solo archivo `.exe` con recursos incrustados.
<img width="600" height="350" alt="ventana" src="https://github.com/user-attachments/assets/0c4d8a9e-8e3b-4c5d-905c-b5950fc15377" />

## Requisitos del Sistema

### Para ejecutar XPatcher v 1.0:
*   Windows 7/8/10/11 (64-bit recomendado).
*   **MinGW-W64 (g++)**: Debe estar instalado y añadido a la variable de entorno `PATH` del sistema para permitir la compilación.

### Para compilar el código fuente (Desarrolladores):
*   Python 3.8+
*   Librerías: `pip install pillow pyinstaller`

## Guía de Uso

1.  **Cargar Archivos:**
    *   Haz clic en **"Cargar Original"** y selecciona el archivo base.
    *   Haz clic en **"Cargar Modificado"** y selecciona la versión actualizada o parcheada.

2.  **Analizar:**
    *   Presiona **"Comparar Archivos"**. El sistema mostrará las diferencias en la ventana de logs.

3.  **Crear Parcheador:**
    *   Ingresa un nombre en el campo "Nombre del parcheador".
    *   Haz clic en **"Generar Ejecutable (.exe)"**.

4.  **Distribuir:**
    *   Se creará un archivo `.exe` (ej. `Actualizacion.exe`). Entrega este archivo a tus usuarios. Al ejecutarlo, solo tendrán que seleccionar el archivo original para aplicarle las actualizaciones.

## Compilación del Proyecto

Si deseas compilar `XPatcher v 1.0` tú mismo, sigue estos pasos:

1.  Asegúrate de tener `logo.png` en la misma carpeta que el script.
2.  Instala las dependencias: `pip install pillow pyinstaller`.
3.  Ejecuta el siguiente comando:

```bash
pyinstaller --noconsole --onefile --add-data "logo.png;." --hidden-import=PIL.Image --hidden-import=PIL._tkinter_finder xpatcher_builder.py
```

## Créditos y Contacto

### Desarrollador Principal
**Rodolfo Hernández BazX**

*   **LinkedIn:** [Perfil de LinkedIn del Programador](https://www.linkedin.com/in/rodolfohbaz/)
*   **Portafolio Personal:** [www.tu-pagina-personal.com](https://rodolfohbaz.info/)

### Empresa Desarrolladora
**[Rhino Forensic & Reverse Toolkit]**

*   **Sitio Web Oficial:** [Rhino Forensic & Reverse Toolkit - 2026](https://rhinosecurity.xyz/)
*   **Soporte:** Rodolfohbaz@gmail.com

---

*Desarrollado con ❤️ y Python.*
```
