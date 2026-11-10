# ProRaw Camera Inspector 1.0

Aplicación Android nativa de diagnóstico Camera2, de solo lectura. No abre el sensor, no captura imágenes, no cambia parámetros del sistema, no requiere root y no solicita permiso CAMERA.

## Qué informa
- IDs de cámara expuestos por CameraManager y, en Android 9+, IDs físicos asociados a cámaras lógicas.
- Nivel de hardware Camera2 y capacidades anunciadas.
- Tamaños de salida RAW_SENSOR y JPEG.
- Rango ISO y rango de exposición en nanosegundos.
- Dimensiones del array de píxeles y área activa.
- Disposición del filtro de color (CFA/Bayer), si se informa.
- Distancia mínima de enfoque, focales, aperturas y modos OIS.

## Compilación
Requiere Android Studio o AndroidIDE con JDK 17, Android SDK Platform 36 y Android Gradle Plugin 8.9.1. Abrir esta carpeta como proyecto Gradle y ejecutar la tarea `app:assembleDebug`. El APK de depuración quedará en `app/build/outputs/apk/debug/app-debug.apk`.

Este paquete entregado es el **proyecto fuente**, no un APK compilado. En el entorno de preparación no hay Android SDK/Gradle instalado para generar y verificar un APK. No se debe instalar como si ya fuera un APK.

## Uso en el teléfono
Instalar el APK generado, abrir la aplicación, esperar el análisis y usar el botón de copiar/seleccionar texto para compartir el informe completo. No se requiere conectar el móvil a un ordenador.
