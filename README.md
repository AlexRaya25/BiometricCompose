# Ejemplo de Autenticación Biométrica en Android con Jetpack Compose

Este proyecto es un ejemplo práctico de cómo implementar la autenticación biométrica (PIN, patrón o contraseña) en una aplicación Android utilizando **Kotlin** y **Jetpack Compose**. La aplicación incluye un flujo básico con dos pantallas: una pantalla de inicio de sesión y una pantalla de inicio, gestionadas mediante **Navigation Compose**.

## Características

- **Autenticación biométrica**: Uso de `BiometricPrompt` para habilitar la autenticación con PIN, patrón o contraseña del dispositivo.
- **Jetpack Compose**: Interfaz de usuario declarativa moderna para Android.
- **Navegación**: Gestión de pantallas y flujo de navegación mediante Navigation Compose.
- Código modular y fácilmente extensible.

## Requisitos

- **Android Studio** Electric Eel o superior.
- **SDK mínimo**: 23 (Android 6.0, Marshmallow).
- **Lenguaje**: Kotlin.

## Instalación

1. Clona este repositorio:
    ```bash
    git clone https://github.com/AlexRaya25/BiometricCompose.git
    ```
2. Abre el proyecto en Android Studio.
3. Sincroniza las dependencias de Gradle.
4. Ejecuta la aplicación en un emulador o dispositivo físico.

## Uso

1. Al iniciar la aplicación, se muestra la pantalla de inicio de sesión.
2. Presiona el botón **"Autenticar"**.
3. Si la autenticación es exitosa, serás redirigido a la pantalla de inicio.
4. En caso de error o autenticación fallida, se mostrará un mensaje informativo.

## Dependencias Clave

```kotlin
dependencies {
    implementation "androidx.compose.ui:ui:1.5.0"               // Jetpack Compose UI
    implementation "androidx.navigation:navigation-compose:2.6.0" // Navigation Compose
    implementation "androidx.biometric:biometric:1.2.0"         // BiometricPrompt API
    implementation "androidx.core:core-ktx:1.12.0"              // Funciones de extensión de Android
    implementation "androidx.activity:activity-compose:1.7.2"   // Compose en actividades
}
