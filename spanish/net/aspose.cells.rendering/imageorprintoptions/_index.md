---
title: "Clase ImageOrPrintOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.ImageOrPrintOptions. Permite especificar opciones al renderizar la hoja de cálculo a imágenes, imprimir la hoja de cálculo o renderizar un gráfico a imagen"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Permite especificar opciones al renderizar la hoja de cálculo a imágenes, imprimir la hoja de cálculo o renderizar un gráfico a imagen.

```csharp
public class ImageOrPrintOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions/)() | Ctor. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de la configuración de página será inválido, y los demás ajustes de la configuración de página seguirán teniendo efecto. |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Indica el tipo de imagen del gráfico al convertir. Valor predeterminado: PNG. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establece una fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo y mostrar estos caracteres primero. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | El cliente puede enviar una salida especial a la impresora al imprimir cada página usando este EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | El cliente puede controlar la configuración de página de la impresora al imprimir cada página usando este EventHandler |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Obtiene o establece configuraciones personalizadas durante el renderizado. |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Obtiene o establece el idioma de edición predeterminado. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establece una fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca la propiedad DefaultFont, como MingLiu o MS Gothic, para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells usará la fuente predeterminada del sistema para mostrar estos caracteres Unicode. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Implemente esta interfaz para obtener DrawObject y Bound al renderizar. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Indica el nombre de archivo de la imagen incrustada en SVG. Debe ser una ruta completa con directorio, por ejemplo "c:\\xpsEmbedded" |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Configuración para renderizar metafiles EMF en el archivo fuente. |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Obtiene o establece un EmfType que especifica el formato del Metafile. El valor predeterminado es EmfPlusDual. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Obtiene o establece el color de la línea de cuadrícula. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Obtiene o establece el tipo de línea de cuadrícula. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Obtiene o establece la resolución horizontal para las imágenes generadas, en puntos por pulgada. |
| virtual [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype/) { get; set; } | Obtiene o establece el formato de las imágenes generadas. Valor predeterminado: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Indica si el ancho y la altura de las celdas se ajustan automáticamente según el valor de la celda. El valor predeterminado es false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con él. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Indica si se deben optimizar los elementos de salida. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de la configuración de página será inválido, y los demás ajustes de la configuración de página seguirán teniendo efecto. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Si esta propiedad es verdadera, se generará una Área y no se aplicará escala. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica si se debe generar una página en blanco cuando no hay nada que imprimir. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Obtiene o establece el número de páginas a guardar. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Obtiene o establece el índice basado en cero de la primera página a guardar. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Controlar/Indicar el progreso del proceso de guardado de la página. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Obtiene o establece el formato de píxel para las imágenes generadas. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Indica qué páginas no se imprimirán. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Si PrintWithStatusDialog = true, aparecerá un diálogo que muestra el estado actual de la impresión. De lo contrario, no se mostrará ningún diálogo. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Obtiene o establece un valor que determina la calidad de las imágenes generadas, aplicable solo al guardar páginas en formato `Jpeg`. El valor predeterminado es 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Obtiene o establece el tipo de formato de archivo de salida. Soporta Tiff/XPS |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Obtiene o establece las hojas a renderizar. Por defecto son todas las hojas visibles en el libro: [`Visible`](../sheetset/visible/). |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Especifica si se aplica suavizado (antialiasing) a líneas y curvas y a los bordes de áreas rellenas. El valor predeterminado es SmoothingMode.None |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) Obtiene y establece el prefijo del nombre css en svg, el valor predeterminado es una cadena vacía. |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) si esta propiedad es verdadera, el svg generado se ajustará al viewport. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Obtiene o establece el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Especifica la calidad del renderizado de texto. El valor predeterminado es TextRenderingHint.SystemDefault |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Obtiene o establece el método usado al convertir imágenes a formato de 1 bpp cuando [`ImageType`](./imagetype/) es Tiff y [`TiffCompression`](./tiffcompression/) es igual a Ccitt3 o Ccitt4. |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Obtiene o establece la profundidad de bits que se aplicará solo al guardar páginas en el formato `Tiff`. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Obtiene o establece el tipo de compresión que se aplicará solo al guardar páginas en el formato `Tiff`. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Indica si el fondo de la imagen generada debe ser transparente. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Obtiene o establece la resolución vertical para las imágenes generadas, en puntos por pulgada. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize)(int, int) | (**Obsolete.**) Establece el ancho y alto deseados de la imagen. |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize_1)(int, int, bool) | Establece el ancho y alto deseados de la imagen. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class RenderingClassImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crea ImageOrPrintOptions y establece sus propiedades
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Crea un nuevo libro con datos de ejemplo y un gráfico
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Guarda el gráfico como imagen usando las opciones
            chart.ToImage("output_chart.png", options);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


