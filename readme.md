# EscribeloYa

Cuaderno digital de escritorio para Windows. Escribe a mano con lápiz o ratón, añade texto, imágenes y figuras en hojas de
tamaño real (A4, A5, A3, Carta), organiza tus cuadernos en una biblioteca y exporta a PDF con las medidas de la hoja.
Funciona sin conexión, sin cuentas y sin telemetría.

Web: [escribeloya.app](https://escribeloya.app)

> **Versión beta.** La aplicación funciona y está probada, pero es una primera versión pública: puede haber fallos.
> Cuéntalos en [Issues](https://github.com/mantiel/escribeloya-releases/issues).

Este repositorio solo contiene los instaladores. El código de la aplicación es privado.

## Descargar

Los instaladores están en [Releases](https://github.com/mantiel/escribeloya-releases/releases). Descarga
`EscribeloYa_<versión>_x64-setup.exe` de la versión más reciente.

| Versión | Estado | SHA-256 del instalador |
|---|---|---|
| 0.1.0-beta.3 | Beta | `6DFA2548CBFDCED9A990D9EB8EFBD21EA818DC6639A8B572A7FFDEC8D660E628` |
| 0.1.0-beta.2 | Beta | `32693C243D8F0D09BC3C1D4C439AC3960C68673BD271581758BC7501649481AB` |
| 0.1.0-beta.1 | Beta | `C43940397F4098FB2652FD0A9FCA125AFC00869581CA87A0B5CB81CCDAF0B1B2` |

## Requisitos

- Windows 10 o 11 de 64 bits.
- WebView2, que ya viene con Windows 10 y 11 actualizados. Si falta, el instalador lo descarga de Microsoft y necesita internet.

## Instalar

1. Ejecuta el instalador. Se instala solo para tu usuario y no pide permisos de administrador.
2. El instalador no está firmado, así que Windows SmartScreen puede mostrar «Windows protegió su PC». Elige
   **Más información** y luego **Ejecutar de todas formas**.

Para comprobar que el archivo es el que se publicó, compara su suma de verificación con la de la tabla (PowerShell):

```powershell
Get-FileHash .\EscribeloYa_0.1.0-beta.3_x64-setup.exe -Algorithm SHA256
```

## Tus datos

Los cuadernos se guardan en tu equipo, en `%APPDATA%\EscribeloYa\notebooks`. Desinstalar la aplicación **no** los borra.
Para llevarlos a otro equipo, crea una copia de seguridad (`.zip`) desde la aplicación y restáurala allí. Nada sale de tu
equipo: la aplicación no hace ninguna conexión.

## Actualizar

No hay actualización automática. Para pasar a una versión nueva, descarga su instalador y ejecútalo: se instala encima de la
anterior y conserva tus cuadernos.

## Lo que aún no está probado

- La impresión a tamaño real (100 %) no se ha medido con una regla. Se exporta a PDF y se imprime desde un lector, sin
  «ajustar a la página».
- La presión del lápiz no se ha probado con un lápiz real.
- Solo Windows 10 y 11 de 64 bits; no hay versión para macOS ni Linux.

## Ayuda y contacto

- Fallos y sugerencias: [Issues](https://github.com/mantiel/escribeloya-releases/issues).
- Correo: contacto@escribeloya.app
