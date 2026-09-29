# MJ Player · REPRODUCTOR HD+

Reproductor de películas para Windows basado en WPF + mpv.

## Versión actual

**v0.6.5 RTX VIDEO**

Incluye Motion², mejora de imagen, HDR, audio avanzado, subtítulos inteligentes, modo portable, integración con Windows, Auto Quality y NVIDIA RTX Video Super Resolution mediante D3D11VPP cuando el hardware/driver lo permiten.

## Descargar

Paquete completo de la versión actual:

[Descargar MJ Player v0.6.5 RTX VIDEO](releases/MJ_Player_v0.6.5_RTX_VIDEO_UN_CLICK.zip)

El ZIP contiene el código fuente, scripts de preparación/compilación, documentación y la configuración portable.

## Ejecución

1. Extraer el ZIP.
2. Ejecutar `EJECUTAR_MJ_PLAYER.bat`.
3. El script prepara mpv y genera la carpeta portable.
4. Luego se puede abrir directamente `MJ_PLAYER_LISTO\MJPlayer.exe`.

## RTX Video

En `Imagen > RTX Video` se puede usar:

- **Off**: desactiva RTX Video.
- **Auto**: lo usa cuando hay GPU NVIDIA RTX y la película realmente necesita reescalado.
- **Forzar**: intenta activarlo cuando la configuración lo permite.

RTX Video Super Resolution y Motion² pesado no se apilan por defecto para evitar una ruta GPU → CPU → GPU innecesaria.

> RTX Video no es DLSS 5. Esta versión usa NVIDIA RTX Video Super Resolution a través de D3D11VPP en mpv.

## Estado del proyecto

Esta rama contiene la versión estable en desarrollo del reproductor. Las siguientes etapas previstas son pruebas RTX reales, compatibilidad/fallback por driver y una futura integración más profunda con NVIDIA Video Effects SDK.
