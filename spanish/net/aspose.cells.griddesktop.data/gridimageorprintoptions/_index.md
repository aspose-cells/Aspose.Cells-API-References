---
title: "Clase GridImageOrPrintOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridDesktop.Data.GridImageOrPrintOptions. Permite especificar opciones al renderizar la hoja de cálculo a imágenes, imprimir la hoja de cálculo o renderizar un gráfico a imagen"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridimageorprintoptions/
---
## GridImageOrPrintOptions class

Permite especificar opciones al renderizar la hoja de cálculo a imágenes, imprimir la hoja de cálculo o renderizar un gráfico a imagen.

```csharp
public class GridImageOrPrintOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridImageOrPrintOptions](gridimageorprintoptions/)() | La construcción de GridImageOrPrintOptions |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de la configuración de página será inválido, y los demás ajustes de la configuración de página seguirán teniendo efecto. |
| [CheckWorkbookDefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establece una fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo y mostrar estos caracteres primero. |
| [DefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/defaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establece una fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca la propiedad DefaultFont, como MingLiu o MS Gothic, para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells usará la fuente predeterminada del sistema para mostrar estos caracteres Unicode. |
| [EmbededImageNameInSvg](../../aspose.cells.griddesktop.data/gridimageorprintoptions/embededimagenameinsvg/) { get; set; } | Indique el nombre de archivo de la imagen incrustada en svg. Esto debe ser la ruta completa con el directorio, como "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/emftype/) { get; set; } | Obtiene o establece un EmfType que especifica el formato del Metafile. El valor predeterminado es EmfPlusDual. |
| [GridlineType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/gridlinetype/) { get; set; } | Obtiene o establece el tipo de línea de cuadrícula. |
| [HorizontalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/horizontalresolution/) { get; set; } | Obtiene o establece la resolución horizontal para las imágenes generadas, en puntos por pulgada. Se aplica al método de generación de imágenes, excepto a imágenes en formato Emf. |
| [ImageType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/imagetype/) { get; set; } | Obtiene o establece el formato de las imágenes generadas. Valor predeterminado: PNG. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con él. |
| [IsOptimized](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isoptimized/) { get; set; } | Indica si se deben optimizar los elementos de salida. |
| [OnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onepagepersheet/) { get; set; } | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de la configuración de página será inválido, y los demás ajustes de la configuración de página seguirán teniendo efecto. |
| [OnlyArea](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onlyarea/) { get; set; } | Si esta propiedad es verdadera, se generará una Área y no se aplicará escala. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica si se debe generar una página en blanco cuando no hay nada que imprimir. |
| [PageCount](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pagecount/) { get; set; } | Obtiene o establece el número de páginas a guardar. |
| [PageIndex](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pageindex/) { get; set; } | Obtiene o establece el índice basado en cero de la primera página a guardar. |
| [PixelFormat](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pixelformat/) { get; set; } | Obtiene o establece el formato de píxel para las imágenes generadas. |
| [PrintingPage](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printingpage/) { get; set; } | Indica qué páginas no se imprimirán. |
| [PrintWithStatusDialog](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printwithstatusdialog/) { get; set; } | Si PrintWithStatusDialog = true, aparecerá un diálogo que muestra el estado actual de la impresión. De lo contrario, no se mostrará ningún diálogo. |
| [Quality](../../aspose.cells.griddesktop.data/gridimageorprintoptions/quality/) { get; set; } | Obtiene o establece un valor que determina la calidad de las imágenes generadas, aplicable solo al guardar páginas en formato `Jpeg`. El valor predeterminado es 100 |
| [SmoothingMode](../../aspose.cells.griddesktop.data/gridimageorprintoptions/smoothingmode/) { get; set; } | Especifica si se aplica suavizado (antialiasing) a líneas y curvas y a los bordes de áreas rellenas. El valor predeterminado es SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.griddesktop.data/gridimageorprintoptions/svgfittoviewport/) { get; set; } | Si esta propiedad es verdadera, el SVG generado se ajustará al viewport. |
| [TextCrossType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textcrosstype/) { get; set; } | Obtiene o establece el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda. |
| [TextRenderingHint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textrenderinghint/) { get; set; } | Especifica la calidad del renderizado de texto. El valor predeterminado es TextRenderingHint.SystemDefault |
| [Transparent](../../aspose.cells.griddesktop.data/gridimageorprintoptions/transparent/) { get; set; } | Indica si el fondo de la imagen generada debe ser transparente. |
| [VerticalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/verticalresolution/) { get; set; } | Obtiene o establece la resolución vertical para las imágenes generadas, en puntos por pulgada. Se aplica al método de generación de imágenes, excepto a imágenes en formato Emf. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setdesiredsize/)(int, int) | Establece el ancho y alto deseados de la imagen. |
| [setRenderSheetSet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setrendersheetset/)(int[]) | Establece las hojas a renderizar. Por defecto son todas las hojas visibles en el libro. Índices de hoja basados en cero. |

### Ver también

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


