---
title: "Clase SvgImageOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.SvgImageOptions. Opciones para generar una imagen Svg"
type: docs
url: /es/net/aspose.cells.rendering/svgimageoptions/
---
## SvgImageOptions class

Opciones para generar una imagen SVG.

```csharp
public class SvgImageOptions : ImageOrPrintOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SvgImageOptions](svgimageoptions/)() | Ctor. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de la configuración de página será inválido, y los demás ajustes de la configuración de página seguirán aplicándose. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Indique el tipo de imagen del gráfico al convertir. Valor predeterminado: PNG. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en PDF o imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo y mostrar estos caracteres primero. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CssPrefix](../../aspose.cells.rendering/svgimageoptions/cssprefix/) { get; set; } | Obtiene y establece el prefijo del nombre CSS en SVG, el valor predeterminado es una cadena vacía. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | El cliente puede realizar una salida especial a la impresora al imprimir cada página usando este EventHandler (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | El cliente puede controlar la configuración de página de la impresora al imprimir cada página usando este EventHandler (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Obtiene o establece configuraciones personalizadas durante el renderizado. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Obtiene o establece el idioma de edición predeterminado. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en PDF o imagen. Establezca la propiedad DefaultFont, como MingLiu o MS Gothic, para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells utilizará la fuente predeterminada del sistema para mostrar estos caracteres Unicode. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Implemente esta interfaz para obtener DrawObject y Bound al renderizar. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmbeddedFontType](../../aspose.cells.rendering/svgimageoptions/embeddedfonttype/) { get; set; } | Obtiene o establece el tipo de fuente que se incrusta en SVG. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Indique el nombre de archivo de la imagen incrustada en SVG. Debe ser una ruta completa con directorio, como "c:\\xpsEmbedded" (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Configuración para renderizar metarchivos EMF en el archivo fuente. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Obtiene o establece un EmfType que especifica el formato del Metarchivo. El valor predeterminado es EmfPlusDual. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [FitToViewPort](../../aspose.cells.rendering/svgimageoptions/fittoviewport/) { get; set; } | Si esta propiedad es verdadera, el SVG generado se ajustará al viewport. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Obtiene o establece el color de la línea de cuadrícula. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Obtiene o establece el tipo de línea de cuadrícula. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Obtiene o establece la resolución horizontal para las imágenes generadas, en puntos por pulgada. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| override [ImageType](../../aspose.cells.rendering/svgimageoptions/imagetype/) { get; set; } | Obtiene o establece el formato de las imágenes generadas. Valor predeterminado: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Indica si el ancho y alto de las celdas se ajustan automáticamente al valor de la celda. El valor predeterminado es false. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con él. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Indica si se deben optimizar los elementos de salida. (Hereda de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de pagesetup será inválido, y los demás ajustes de pagesetup seguirán teniendo efecto. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Si esta propiedad es verdadera, se exportará una Área, y ninguna escala tendrá efecto. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica si se debe exportar una página en blanco cuando no hay nada que imprimir. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Obtiene o establece el número de páginas a guardar. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Obtiene o establece el índice basado en cero de la primera página a guardar. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Controla/Indica el progreso del proceso de guardado de páginas. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Obtiene o establece el formato de píxel para las imágenes generadas. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Indica qué páginas no se imprimirán. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Si PrintWithStatusDialog = true, aparecerá un diálogo que muestra el estado de impresión actual. De lo contrario, no se mostrará dicho diálogo. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Obtiene o establece un valor que determina la calidad de las imágenes generadas, aplicable solo al guardar páginas en formato `Jpeg`. El valor predeterminado es 100(Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsoleto.**) Obtiene o establece el tipo de formato de archivo de salida Soporta Tiff/XPS(Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Obtiene o establece las hojas a renderizar. El valor predeterminado es todas las hojas visibles en el libro de trabajo: [`Visible`](../sheetset/visible/). (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Especifica si se aplica suavizado (antialiasing) a líneas y curvas y a los bordes de áreas rellenas. El valor predeterminado es SmoothingMode.None(Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsoleto.**) Obtiene y establece el prefijo del nombre css en svg, el valor predeterminado es una cadena vacía. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsoleto.**) Si esta propiedad es verdadera, el svg generado se ajustará al viewport. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Obtiene o establece el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Especifica la calidad del renderizado de texto. El valor predeterminado es TextRenderingHint.SystemDefault(Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Obtiene o establece el método usado al convertir imágenes al formato de 1 bpp cuando [`ImageType`](../imageorprintoptions/imagetype/) es Tiff y [`TiffCompression`](../imageorprintoptions/tiffcompression/) es igual a Ccitt3 o Ccitt4. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Obtiene o establece la profundidad de bits a aplicar solo al guardar páginas en formato `Tiff`. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Obtiene o establece el tipo de compresión a aplicar solo al guardar páginas en formato `Tiff`. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Indica si el fondo de la imagen generada debe ser transparente. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Obtiene o establece la resolución vertical para las imágenes generadas, en puntos por pulgada. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int) | (**Obsoleto.**) Establece el ancho y alto deseados de la imagen. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int, bool) | Establece el ancho y alto deseados de la imagen. (Heredado de [`ImageOrPrintOptions`](../imageorprintoptions/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassSvgImageOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(12000);
            worksheet.Cells["A3"].PutValue(16500);
            worksheet.Cells["B1"].PutValue("Q2");
            worksheet.Cells["B2"].PutValue(25500);
            worksheet.Cells["B3"].PutValue(10800);

            // Crear un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Inicializar opciones de imagen SVG
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Configurar opciones de renderizado SVG
            svgOptions.FitToViewPort = true;
            svgOptions.CssPrefix = "chart-";
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;
            svgOptions.ImageType = ImageType.Svg;

            // Establecer la calidad de impresión y la resolución
            svgOptions.PrintWithStatusDialog = true;
            svgOptions.HorizontalResolution = 300;
            svgOptions.VerticalResolution = 300;

            // Renderizar el gráfico a SVG con las opciones configuradas
            chart.ToImage("chart_output.svg", svgOptions);

            // Demostrar la integración de guardado del libro de trabajo
            workbook.Save("SvgRenderingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../imageorprintoptions/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


