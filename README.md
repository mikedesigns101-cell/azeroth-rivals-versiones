# Azeroth Rivals · versiones

**Azeroth Rivals** es un juego de peleas por equipos con cámara cenital, ambientado en Warcraft.
Está en **alpha**: lo estamos probando entre amigos, así que habrá fallos, cosas sin terminar y cambios
de una versión a otra.

Este repositorio solo guarda las versiones para descargar. El código del juego no está aquí.

> Proyecto de aficionados, no oficial: no tiene relación con Blizzard Entertainment ni cuenta con su
> respaldo. Warcraft y World of Warcraft son marcas de Blizzard Entertainment, Inc.

## Qué necesitas

- Windows 10 u 11 de 64 bits.
- Una tarjeta gráfica compatible con Vulkan (casi cualquiera de los últimos años).
- Unos 250 MB libres: el juego ocupa unos 120 MB y, mientras se actualiza, guarda la versión nueva al lado.

## Cómo se instala

1. Entra en la [última versión](https://github.com/mikedesigns101-cell/azeroth-rivals-versiones/releases/latest)
   y descarga **AzerothRivals.exe**. El resto de archivos no hacen falta: el `.sha256` sirve para comprobar
   la descarga y «Source code» lo añade GitHub solo (aquí no hay código).
2. Crea una carpeta para el juego, por ejemplo `Documentos\Azeroth Rivals` o `D:\Juegos\Azeroth Rivals`, y
   mueve el exe allí. Mejor que no sea `Archivos de programa` ni `Descargas`: en la primera Windows no deja que
   el juego se actualice solo, y en la segunda es fácil borrarlo sin querer.
3. Ábrelo con doble clic. No hay instalador ni hace falta nada más.

## El aviso de Windows (SmartScreen)

La primera vez que lo abras, Windows puede enseñar una pantalla azul que dice **«Windows protegió su PC»**.
Sale porque el exe no está firmado con un certificado (cuestan dinero y esto es una alpha entre amigos), no
porque se haya encontrado nada en él.

Para abrirlo: pulsa **Más información** y luego **Ejecutar de todas formas**. Pasa con el exe que bajas con el
navegador; las versiones que descarga el propio juego normalmente no lo piden.

Si el navegador avisa al descargarlo de que «no se descarga habitualmente», elige **Conservar**.

¿Quieres comprobar que el archivo es el publicado? En PowerShell, dentro de la carpeta del juego:

```
Get-FileHash .\AzerothRivals.exe
```

El resultado tiene que ser el mismo que el del archivo `AzerothRivals.exe.sha256` de esa versión.

## Actualizaciones

Al abrirse, el juego mira si hay una versión nueva aquí. Si la hay, en el menú aparece un aviso con lo que
cambia:

- **Actualizar**: la descarga, comprueba que ha llegado entera y sin cambios, y vuelve a abrir el juego ya
  actualizado. Se puede cancelar mientras descarga.
- **Más tarde**: no vuelve a avisar hasta la próxima vez que abras el juego.

Para saberlo solo pregunta a GitHub cuál es la última versión publicada en este repositorio. No envía nada
tuyo. Sin internet, el juego funciona igual y no avisa de nada.

Si la carpeta del juego no deja guardar archivos, el aviso ofrece abrir esta página para que la bajes a mano.
Las versiones anteriores al actualizador (la 0.5.0 y las de antes) no lo traen: esa vez hay que bajar la
nueva a mano y sustituir el exe.

## Si algo falla

En partida, **F8** guarda un aviso con una captura y la partida para poder verla otra vez. En el menú,
**Abrir carpeta de avisos** te lleva a ellos: comprime la carpeta y compártela en el grupo.
