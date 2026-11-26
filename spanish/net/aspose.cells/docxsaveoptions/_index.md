---
title: "Clase DocxSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DocxSaveOptions. Representa opciones de guardado de archivos .docx"
type: docs
url: /es/net/aspose.cells/docxsaveoptions/
---
## DocxSaveOptions class

Representa las opciones para guardar un archivo .docx.

```csharp
public class DocxSaveOptions : PaginatedSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DocxSaveOptions](docxsaveoptions/#constructor)() | Representa las opciones para guardar un archivo .docx. |
| [DocxSaveOptions](docxsaveoptions/#constructor_1)(bool) | Representa las opciones para guardar un archivo .docx. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de la configuración de página será ignorado, y los demás ajustes de la configuración de página seguirán teniendo efecto. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [AsFlatOpc](../../aspose.cells/docxsaveoptions/asflatopc/) { get; set; } | Indica si se guarda como un archivo opc plano que puede ser generado por Open XML SDK |
| [AsNormalView](../../aspose.cells/docxsaveoptions/asnormalview/) { get; set; } | Exportando archivo de Excel a docx como vista normal. Si esta propiedad es verdadera, se generará una Área y no se aplicará escala. El valor predeterminado es falso. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando se ingresa un valor más largo que 32K, se truncará.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Indica si se debe comprobar la compatibilidad de fuentes para cada carácter en el texto. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establecen con la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo para mostrar estos caracteres primero. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dejar el libro de trabajo vacío después de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Obtiene o establece configuraciones personalizadas durante la renderización. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Obtiene o establece el idioma de edición predeterminado. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | Cuando los caracteres en el Excel son Unicode y no se establecen con la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca la DefaultFont, como MingLiu o MS Gothic, para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells usará la fuente predeterminada del sistema para mostrar estos caracteres Unicode. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implementa esta interfaz para obtener DrawObject y Bound al renderizar. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedXlsxAsChartDataSource](../../aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/) { get; set; } | Indica si se incrusta un archivo xlsx como fuente de datos del gráfico. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Configuración para renderizar metafile Emf. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Obtiene o establece el color de la línea de cuadrícula. (Heredado de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Obtiene o establece el tipo de línea de cuadrícula.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Indica si necesita ocultar el error durante la renderización. El error puede ser un error en forma, imagen, renderizado de gráfico, etc.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica si solo se sustituye la fuente del carácter cuando la fuente de la celda no es compatible con ella.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de la configuración de página será inválido, y los demás ajustes de la configuración de página seguirán teniendo efecto.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica si se debe generar una página en blanco cuando no hay nada que imprimir.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Obtiene o establece el número de páginas a guardar.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Obtiene o establece el índice basado en cero de la primera página a guardar.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Controla/Indica el progreso del proceso de guardado de páginas.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Indica qué páginas no se imprimirán.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Obtiene o establece los comportamientos de renderizado específicos de Excel a aplicar.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveAsEditableShapes](../../aspose.cells/docxsaveoptions/saveaseditableshapes/) { get; set; } | Guarda todos los objetos de dibujo como formas editables en el archivo de Word, para que puedas editarlos en Word. |
| [SaveAsEditableShaps](../../aspose.cells/docxsaveoptions/saveaseditableshaps/) { get; set; } | (**Obsoleto.**) Guarda todos los objetos de dibujo como formas editables en el archivo de Word. Así puedes editarlos en Word. |
| [SaveElementType](../../aspose.cells/docxsaveoptions/saveelementtype/) { get; set; } | Indica qué elementos deben guardarse. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Obtiene o establece las hojas a renderizar. El valor predeterminado son todas las hojas visibles en el libro: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Obtiene o establece el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda.(Hereda de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
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

    public class DocxSaveOptionsDemo
    {
        public static void DocxSaveOptionsExample()
        {
            // Abre un archivo de Excel
            Workbook workbook = new Workbook("DocxSaveOptions_original.xlsx");

            // Crea una instancia de DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();

            // Estableciendo propiedades
            saveOptions.DefaultFont = "MS Gothic";
            saveOptions.CheckWorkbookDefaultFont = true;
            saveOptions.CheckFontCompatibility = false;
            saveOptions.IsFontSubstitutionCharGranularity = true;
            saveOptions.OnePagePerSheet = true;
            saveOptions.AllColumnsInOnePagePerSheet = false;
            saveOptions.IgnoreError = true;
            saveOptions.OutputBlankPageWhenNothingToPrint = false;
            saveOptions.PageIndex = 0;  // Starting page index (0-based index)
            saveOptions.PageCount = 2;  // Number of pages to be printed
            saveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            saveOptions.GridlineType = GridlineType.Dotted;
            saveOptions.TextCrossType = TextCrossType.CrossKeep;
            saveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
            saveOptions.SheetSet = SheetSet.All;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = @"C:\Cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = false;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Guarda el documento en formato DOCX
            workbook.Save("DocxSaveOptionsExample.docx", saveOptions);

            return;
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


