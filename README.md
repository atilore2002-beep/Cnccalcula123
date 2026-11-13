# CNC Calculadora Pro — proyecto Android

Proyecto inicial Android nativo en Kotlin + Jetpack Compose para torno CNC FANUC.

## Incluye en esta primera versión
- Pantalla principal.
- Cálculo de RPM a partir de Vc y diámetro.
- Cálculo de avance en mm/min.
- Cálculo geométrico de conos.
- Estimación teórica de rosca métrica exterior ISO.
- Referencia rápida de códigos G/M FANUC.

## Abrir
1. Descomprime el ZIP.
2. Abre Android Studio.
3. Selecciona Open y elige la carpeta `CNCCalculadoraPro`.
4. Espera a que termine la sincronización de Gradle.
5. Ejecuta en un emulador o móvil Android.

## Generar APK
En Android Studio: Build > Build Bundle(s) / APK(s) > Build APK(s).

## Importante
Es una primera versión funcional de cálculo, no una validación de proceso. Verifica siempre fórmulas, unidades, tolerancias, sintaxis específica de control y condiciones de máquina. Simula y valida cualquier programa antes de ejecutarlo en una máquina real.


## Compilación desde un móvil mediante GitHub Actions

Este proyecto incluye `.github/workflows/android-build.yml`. Al subir el proyecto a un repositorio GitHub,
la acción compilará un APK de depuración. En GitHub abre la pestaña **Actions**, selecciona
**Build CNC Calculadora Pro APK** y, al terminar correctamente, descarga el artefacto
**CNC-Calculadora-Pro-debug**. Dentro estará `app-debug.apk`.

Nota: esta compilación en la nube no se ha ejecutado ni verificado todavía. El APK de depuración
es para pruebas personales, no una versión firmada para publicar. Antes de usar cualquier
cálculo o programa CNC en una máquina real, comprueba los resultados y simula el programa.
