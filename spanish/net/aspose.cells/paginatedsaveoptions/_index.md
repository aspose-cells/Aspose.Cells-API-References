---
title: "Clase PaginatedSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.PaginatedSaveOptions. Representa las opciones para la paginación"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/
---
## PaginatedSaveOptions class

Representa las opciones de paginación.

```csharp
public abstract class PaginatedSaveOptions : SaveOptions
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de la configuración de página será ignorado, y los demás ajustes de la configuración de página seguirán teniendo efecto. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando se ingresa un valor más largo que 32K, se truncará.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Indica si se debe comprobar la compatibilidad de fuentes para cada carácter en el texto. |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establece una fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo y mostrar estos caracteres primero. |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dejar el libro de trabajo vacío después de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Obtiene o establece configuraciones personalizadas durante el renderizado. |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Obtiene o establece el idioma de edición predeterminado. |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establece una fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca la propiedad DefaultFont, como MingLiu o MS Gothic, para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells usará la fuente predeterminada del sistema para mostrar estos caracteres Unicode. |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implemente esta interfaz para obtener DrawObject y Bound al renderizar. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Configuración para renderizar metarchivo Emf. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Obtiene o establece el color de la línea de cuadrícula. |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Obtiene o establece el tipo de línea de cuadrícula. |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Indica si necesita ocultar el error durante el renderizado. El error puede ser un error en la forma, imagen, renderizado de gráfico, etc. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con él. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de la configuración de página será inválido, y los demás ajustes de la configuración de página seguirán teniendo efecto. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica si se debe generar una página en blanco cuando no hay nada que imprimir. |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Obtiene o establece el número de páginas a guardar. |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Obtiene o establece el índice basado en cero de la primera página a guardar. |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Controlar/Indicar el progreso del proceso de guardado de la página. |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Indica qué páginas no se imprimirán. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Obtiene o establece los comportamientos de renderizado específicos de Excel a aplicar. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Obtiene o establece las hojas a renderizar. Por defecto son todas las hojas visibles en el libro: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Obtiene o establece el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de SmartArt. El valor predeterminado es falso.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. (Hereda de [`SaveOptions`](../saveoptions/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsDemo
    {
        public static void PaginatedSaveOptionsExample()
        {
            // Abre un archivo de Excel
            Workbook workbook = new Workbook("PaginatedSaveOptionsExample_original.xlsx");

            // Crear una instancia de PaginatedSaveOptions
            PdfSaveOptions options = new PdfSaveOptions();

            // Estableciendo propiedades
            options.DefaultFont = "Arial";
            options.CheckWorkbookDefaultFont = true;
            options.CheckFontCompatibility = true;
            options.IsFontSubstitutionCharGranularity = true;
            options.OnePagePerSheet = false;
            options.AllColumnsInOnePagePerSheet = false;
            options.IgnoreError = true;
            options.OutputBlankPageWhenNothingToPrint = false;
            options.PageIndex = 3; // Starting page index (0-based index)
            options.PageCount = 2; // Number of pages to be printed
            options.PrintingPageType = PrintingPageType.IgnoreBlank;
            options.GridlineType = GridlineType.Dotted;
            options.TextCrossType = TextCrossType.CrossKeep;
            options.DefaultEditLanguage = DefaultEditLanguage.English;
            options.SheetSet = new SheetSet(new int[] { workbook.Worksheets.ActiveSheetIndex });
            options.ClearData = false;
            options.CachedFileFolder = "C:\\Temp";
            options.ValidateMergedAreas = true;
            options.MergeAreas = true;
            options.SortNames = true;
            options.SortExternalNames = true;
            options.RefreshChartCache = true;
            options.UpdateSmartArt = false;

            // Guardar el archivo PDF
            workbook.Save("PaginatedSaveOptionsExample.pdf", options);

            return;
        }
    }
}
```

### Ver también

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


