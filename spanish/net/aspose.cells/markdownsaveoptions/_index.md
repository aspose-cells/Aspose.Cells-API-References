---
title: "Clase MarkdownSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.MarkdownSaveOptions clase. Representa las opciones de guardado para markdown"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/
---
## MarkdownSaveOptions class

Representa las opciones de guardado para markdown.

```csharp
public class MarkdownSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [MarkdownSaveOptions](markdownsaveoptions/)() | Crea opciones para guardar el documento markdown |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlignColumnPadding](../../aspose.cells/markdownsaveoptions/aligncolumnpadding/) { get; set; } | Indica si la alineación de columnas está habilitada para las tablas Markdown generadas. Cuando está habilitada, las columnas se alinean rellenando el contenido de la celda con el carácter especificado (normalmente ' ' para espacios). Establezca '\0' para desactivar la alineación de columnas (valor predeterminado). |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/markdownsaveoptions/calculateformula/) { get; set; } | Indica si se deben calcular las fórmulas antes de guardar el archivo markdown. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando se ingresa un valor más largo que 32K, se truncará.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dejar el libro de trabajo vacío después de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/markdownsaveoptions/encoding/) { get; set; } | Obtiene y establece la codificación predeterminada. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ExportHyperlinkAsReference](../../aspose.cells/markdownsaveoptions/exporthyperlinkasreference/) { get; set; } | Indica si se debe exportar el hipervínculo usando definiciones de referencia en lugar del formato en línea. El valor predeterminado es falso. |
| [ExportImagesAsBase64](../../aspose.cells/markdownsaveoptions/exportimagesasbase64/) { get; set; } | Especifica si las imágenes se guardan en formato Base64 en Markdown. El valor predeterminado es verdadero. |
| [FormatStrategy](../../aspose.cells/markdownsaveoptions/formatstrategy/) { get; set; } | Obtiene y establece la estrategia de formato al exportar el valor de la celda como cadena. |
| [ImageOptions](../../aspose.cells/markdownsaveoptions/imageoptions/) { get; } | Obtenga el objeto ImageOrPrintOptions antes de exportar |
| [LightCellsDataProvider](../../aspose.cells/markdownsaveoptions/lightcellsdataprovider/) { get; set; } | El proveedor de datos para proporcionar datos de celdas al guardar el libro de trabajo en modo ligero. |
| [LineSeparator](../../aspose.cells/markdownsaveoptions/lineseparator/) { get; set; } | Obtiene y establece el separador de línea. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [OfficeMathOutputType](../../aspose.cells/markdownsaveoptions/officemathoutputtype/) { get; set; } | Indica cómo se exportan los objetos OfficeMath a Markdown, el valor predeterminado es Imagen. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/markdownsaveoptions/sheetset/) { get; set; } | Obtiene o establece las hojas a renderizar. El valor predeterminado son todas las hojas visibles en el libro de trabajo: [`Active`](../../aspose.cells.rendering/sheetset/active/). |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SplitTablesByBlankRow](../../aspose.cells/markdownsaveoptions/splittablesbyblankrow/) { get; set; } | Indica si las filas en blanco en la hoja de cálculo deben tratarse como separadores de tabla al exportar a Markdown. El valor predeterminado es falso. |
| [StreamProvider](../../aspose.cells/markdownsaveoptions/streamprovider/) { get; set; } | Obtiene o establece el IStreamProvider para exportar objetos. Si `null`, los objetos exportados se guardarán en el mismo directorio que el archivo de salida. |
| [TableHeaderType](../../aspose.cells/markdownsaveoptions/tableheadertype/) { get; set; } | Obtiene y establece cómo definir el encabezado de la tabla. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de SmartArt. El valor predeterminado es falso.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. (Hereda de [`SaveOptions`](../saveoptions/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class MarkdownSaveOptionsDemo
    {
        public static void MarkdownSaveOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Crea una instancia de MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = "\n",
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Guarda el libro de trabajo como un archivo Markdown
            workbook.Save("MarkdownSaveOptionsExample.md", saveOptions);

            Console.WriteLine("Workbook saved as Markdown file successfully.");
        }
    }
}
```

### Ver también

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


