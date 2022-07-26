---
title: ImageOrPrintOptions
second_title: Referencia de API de Aspose.Cells para .NET
description: Permite especificar opciones al representar la hoja de trabajo en imágenes imprimir la hoja de trabajo o representar el gráfico en la imagen.
type: docs
weight: 5140
url: /es/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Permite especificar opciones al representar la hoja de trabajo en imágenes, imprimir la hoja de trabajo o representar el gráfico en la imagen.

```csharp
public class ImageOrPrintOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet) { get; set; } | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de la columna de una hoja se generará en una sola página como resultado. El ancho del tamaño del papel de configuración de página no será válido, y las demás configuraciones de configuración de página seguirán teniendo efecto. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont) { get; set; } | Cuando los caracteres en Excel son Unicode y no están configurados con la fuente correcta en el estilo de celda, Pueden aparecer como bloque en pdf,imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar estos caracteres primero. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler) { get; set; } | El cliente puede enviar una salida especial a la impresora cuando imprime cada página usando este EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler) { get; set; } | El cliente puede controlar la configuración de página de la impresora cuando imprime cada página usando este EventHandler |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage) { get; set; } | Obtiene o establece el idioma de edición predeterminado. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont) { get; set; } | Cuando los caracteres en Excel son Unicode y no están configurados con la fuente correcta en el estilo de celda, Pueden aparecer como bloque en pdf, imagen. Establezca la Fuente predeterminada como MingLiu o MS Gothic para mostrar estos caracteres. Si esta propiedad es no configurado, Aspose.Cells utilizará la fuente predeterminada del sistema para mostrar estos caracteres Unicode. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler) { get; set; } | Implementa esta interfaz para obtener DrawObject y Bound al renderizar. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg) { get; set; } | Indique el nombre de archivo de la imagen incrustada en svg. Esta debería ser la ruta completa con un directorio como "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype) { get; set; } | Obtiene o establece un EmfType que especifica el formato del Metafile.. El valor predeterminado es EmfPlusDual. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype) { get; set; } | Obtiene o establece el tipo de línea de cuadrícula. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution) { get; set; } | Obtiene o establece la resolución horizontal de las imágenes generadas, en puntos por pulgada. Aplica el método de generación de imágenes excepto las imágenes en formato Emf. |
| [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype) { get; set; } | Obtiene o establece el formato de las imágenes generadas. valor por defecto: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit) { get; set; } | Indica si el ancho y el alto de las celdas se ajusta automáticamente por valor de celda. El valor por defecto es false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity) { get; set; } | Indica si solo se sustituye la fuente del carácter cuando la fuente de la celda no es compatible con él. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized) { get; set; } | Indica si optimizar los elementos de salida. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet) { get; set; } | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se generará en una sola página como resultado. El tamaño de papel de la configuración de la página no será válido y las demás configuraciones de la configuración de la página seguirán teniendo efecto. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea) { get; set; } | Si esta propiedad es verdadera, se generará un área y no tendrá efecto ninguna escala. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint) { get; set; } | Indica si se imprime una página en blanco cuando no hay nada que imprimir. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount) { get; set; } | Obtiene o establece el número de páginas a guardar. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex) { get; set; } | Obtiene o establece el índice basado en 0 de la primera página para guardar. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback) { get; set; } | Controlar/Indicar el progreso del proceso de guardado de página. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat) { get; set; } | Obtiene o establece el formato de píxeles de las imágenes generadas. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage) { get; set; } | Indica qué páginas no se imprimirán. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog) { get; set; } | Si PrintWithStatusDialog = true, habrá un cuadro de diálogo que muestra el estado de impresión actual. de lo contrario, no se mostrará dicho cuadro de diálogo. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality) { get; set; } | Obtiene o establece un valor que determina la calidad de las imágenes generadas para aplicar solo al guardar páginas en el`JPEG` formato. El valor predeterminado es 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat) { get; set; } | Obtiene o establece el formato del archivo de salida type Admite Tiff/XPS |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode) { get; set; } | Especifica si se aplica suavizado (antialiasing) a las líneas y curvas y los bordes de las áreas rellenas. El valor predeterminado es SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport) { get; set; } | si esta propiedad es verdadera, el svg generado se ajustará al puerto de vista. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype) { get; set; } | Obtiene o establece el tipo de texto que se muestra cuando el ancho del texto es mayor que el ancho de la celda. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint) { get; set; } | Especifica la calidad de la representación del texto. El valor predeterminado es TextRenderingHint.SystemDefault |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth) { get; set; } | Obtiene o establece la profundidad de bits para que se aplique solo al guardar páginas en el`Pelea` formato. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression) { get; set; } | Obtiene o establece el tipo de compresión que se aplicará solo al guardar páginas en el`Pelea` formato. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent) { get; set; } | Indica si el fondo de la imagen generada debe ser transparente. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution) { get; set; } | Obtiene o establece la resolución vertical de las imágenes generadas, en puntos por pulgada. Aplica el método de generación de imágenes, excepto la imagen en formato Emf. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize)(int, int) | Establece el ancho y el alto deseados de la imagen. |

### Ejemplos

```csharp

[C#]

//Establecer imagen o opciones de impresión
ImageOrPrintOptions options = new ImageOrPrintOptions();

//Establece el formato de la imagen de salida
options.ImageType = ImageType.Png;

//Establecer resolución horizontal
options.HorizontalResolution = 300;

//Establecer resolución vertical
options.VerticalResolution = 300;

//Instanciar libro de trabajo
Workbook book = new Workbook("test.xls");

//Guardar gráfico como imagen usando las opciones ImageOrPrint
book.Worksheets[0].Charts[0].ToImage("chart.png", options);

[VB.NET]

'Establecer imagen o opciones de impresión
Dim options As New ImageOrPrintOptions()

'Establecer formato de imagen de salida
options.ImageType = ImageType.Png

'Establecer resolución horizontal
options.HorizontalResolution = 300

'Establecer resolución vertical
options.VerticalResolution = 300

'Instanciar libro de trabajo
Dim book As New Workbook("test.xls")

'Guardar gráfico como imagen usando las opciones de ImageOrPrint
book.Worksheets(0).Charts(0).ToImage("chart.png", options)
```

### Ver también

* espacio de nombres [Aspose.Cells.Rendering](../../aspose.cells.rendering)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
