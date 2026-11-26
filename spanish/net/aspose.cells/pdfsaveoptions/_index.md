---
title: "Clase PdfSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.PdfSaveOptions. Representa las opciones para guardar un archivo pdf"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Representa las opciones para guardar un archivo PDF.

```csharp
public class PdfSaveOptions : PaginatedSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Crea las opciones para guardar un archivo pdf. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de la configuración de página será ignorado, y los demás ajustes de la configuración de página seguirán teniendo efecto. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark/) { get; set; } | Obtiene y establece el objeto [`PdfBookmarkEntry`](../../aspose.cells.rendering/pdfbookmarkentry/). |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula/) { get; set; } | Indica si se deben calcular las fórmulas antes de guardar el archivo pdf. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando se ingresa un valor más largo que 32K, se truncará.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Indica si se debe comprobar la compatibilidad de fuentes para cada carácter en el texto. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establecen con la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar estos caracteres primero. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dejar el libro de trabajo vacío después de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance/) { get; set; } | Obtiene o establece el nivel de cumplimiento de normas PDF para los documentos de salida. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime/) { get; set; } | Obtiene o establece la hora de generación del documento pdf. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport/) { get; set; } | Obtiene o establece un valor que determina la forma en que [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) se exportan al archivo PDF. El valor predeterminado es Ninguno. |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Obtiene o establece configuraciones personalizadas durante la renderización. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Obtiene o establece el idioma de edición predeterminado. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establecen con la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca la DefaultFont, como MingLiu o MS Gothic, para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells usará la fuente predeterminada del sistema para mostrar estos caracteres Unicode. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle/) { get; set; } | Indica si la barra de título de la ventana debe mostrar el título del documento. |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implementa esta interfaz para obtener DrawObject y Bound al renderizar. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedAttachments](../../aspose.cells/pdfsaveoptions/embedattachments/) { get; set; } | Indica si se debe incrustar el adjunto para objetos Ole en Excel. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/) { get; set; } | True para incrustar fuentes TrueType. Afecta solo a los caracteres ASCII 32-127. Las fuentes para códigos de carácter mayores a 127 siempre se incrustan. Las fuentes siempre se incrustan para el estándar PDF/A-1a, PDF/A-1b. El valor predeterminado es true. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Configuración para renderizar metafile Emf. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure/) { get; set; } | Indica si se debe exportar la estructura del documento. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding/) { get; set; } | Obtiene o establece la codificación de fuentes incrustadas en pdf. |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Obtiene o establece el color de la línea de cuadrícula. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Obtiene o establece el tipo de línea de cuadrícula.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Indica si necesita ocultar el error durante la renderización. El error puede ser un error en forma, imagen, renderizado de gráfico, etc.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ImageType](../../aspose.cells/pdfsaveoptions/imagetype/) { get; set; } | (**Obsolete.**) Representa el tipo de imagen al convertir el gráfico y la forma. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica si solo se sustituye la fuente del carácter cuando la fuente de la celda no es compatible con ella.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de la configuración de página será inválido, y los demás ajustes de la configuración de página seguirán teniendo efecto.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype/) { get; set; } | Obtiene y establece el tipo de optimización pdf. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica si se debe generar una página en blanco cuando no hay nada que imprimir.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Obtiene o establece el número de páginas a guardar.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Obtiene o establece el índice basado en cero de la primera página a guardar.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Controla/Indica el progreso del proceso de guardado de páginas.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression/) { get; set; } | Indica el algoritmo de compresión |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Indica qué páginas no se imprimirán.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Producer](../../aspose.cells/pdfsaveoptions/producer/) { get; set; } | Obtiene y establece el productor del documento pdf generado. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Obtiene o establece los comportamientos de renderizado específicos de Excel a aplicar.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions/) { get; set; } | Establece estas opciones, cuando se necesita seguridad en el resultado xls2pdf. |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Obtiene o establece las hojas a renderizar. El valor predeterminado son todas las hojas visibles en el libro: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Obtiene o establece el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de SmartArt. El valor predeterminado es falso.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. (Hereda de [`SaveOptions`](../saveoptions/).) |
| [Watermark](../../aspose.cells/pdfsaveoptions/watermark/) { get; set; } | Obtiene o establece la marca de agua para la salida. |
| [ZoomBehavior](../../aspose.cells/pdfsaveoptions/zoombehavior/) { get; set; } | Obtiene o establece el modo de vista inicial cuando se abre el documento PDF generado. El valor predeterminado es Ninguno. |
| [ZoomFactor](../../aspose.cells/pdfsaveoptions/zoomfactor/) { get; set; } | Obtiene o establece el porcentaje de zoom usado cuando [`ZoomBehavior`](./zoombehavior/) es ZoomFactor. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample/)(int, int) | Establece el PPI(píxeles por pulgada) deseado para el remuestreo de imágenes y la calidad JPEG. Todas las imágenes se convertirán a JPEG con la configuración de calidad especificada, y las imágenes que superen el PPI especificado (píxeles por pulgada) serán remuestreadas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Rendering.PdfSecurity;
    using System;
    using System.Drawing;

    public class PdfSaveOptionsDemo
    {
        public static void PdfSaveOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Save Options Example");

            // Crea una instancia de PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Establece varias propiedades
            pdfSaveOptions.EmbedStandardWindowsFonts = true;
            pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
            pdfSaveOptions.CalculateFormula = true;
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate;
            pdfSaveOptions.CreatedTime = DateTime.Now;
            pdfSaveOptions.Producer = "Aspose.Cells";
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;
            pdfSaveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;
            pdfSaveOptions.ExportDocumentStructure = true;
            pdfSaveOptions.DisplayDocTitle = true;
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.EmbedAttachments = true;
            pdfSaveOptions.DefaultFont = "Arial";
            pdfSaveOptions.CheckWorkbookDefaultFont = true;
            pdfSaveOptions.CheckFontCompatibility = true;
            pdfSaveOptions.IsFontSubstitutionCharGranularity = true;
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;
            pdfSaveOptions.IgnoreError = true;
            pdfSaveOptions.OutputBlankPageWhenNothingToPrint = true;
            pdfSaveOptions.PageIndex = 0;
            pdfSaveOptions.PageCount = 1;
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            pdfSaveOptions.GridlineType = GridlineType.Dotted;
            pdfSaveOptions.TextCrossType = TextCrossType.CrossKeep;
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.English;
            pdfSaveOptions.SheetSet = SheetSet.Visible;
            pdfSaveOptions.ClearData = true;
            pdfSaveOptions.CachedFileFolder = "C:\\Temp";
            pdfSaveOptions.ValidateMergedAreas = true;
            pdfSaveOptions.MergeAreas = true;
            pdfSaveOptions.SortNames = true;
            pdfSaveOptions.SortExternalNames = true;
            pdfSaveOptions.RefreshChartCache = true;

            // Establece opciones de seguridad
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions
            {
                OwnerPassword = "OwnerPassword",
                UserPassword = "UserPassword",
                PrintPermission = true,
                FullQualityPrintPermission = true
            };
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Establece marca de agua
            RenderingFont font = new RenderingFont("Calibri", 68)
            {
                Italic = true,
                Bold = true,
                Color = Color.Blue
            };
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Rotation = 30,
                Opacity = 0.6f,
                ScaleToPagePercent = 50
            };
            pdfSaveOptions.Watermark = watermark;

            // Guarda el libro de trabajo como un archivo PDF
            workbook.Save("PdfSaveOptionsExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


