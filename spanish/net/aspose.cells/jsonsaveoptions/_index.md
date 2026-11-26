---
title: "Clase JsonSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.JsonSaveOptions. Representa las opciones de guardar el libro de trabajo como un archivo JSON"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/
---
## JsonSaveOptions class

Representa las opciones de guardar el libro de trabajo como un archivo JSON.

```csharp
public class JsonSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [JsonSaveOptions](jsonsaveoptions/)() | Crea opciones para guardar el archivo json. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlwaysExportAsJsonObject](../../aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/) { get; set; } | Indica si siempre se exporta excel a json como objeto, incluso cuando solo hay una hoja de cálculo en el archivo. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando se ingresa un valor más largo que 32K, se truncará.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dejar el libro de trabajo vacío después de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ExportArea](../../aspose.cells/jsonsaveoptions/exportarea/) { get; set; } | Obtiene o establece el rango de exportación. |
| [ExportAsString](../../aspose.cells/jsonsaveoptions/exportasstring/) { get; set; } | Exporta el valor de cadena de las celdas a json. |
| [ExportEmptyCells](../../aspose.cells/jsonsaveoptions/exportemptycells/) { get; set; } | Indica si se exportan celdas vacías como null. |
| [ExportHyperlinkType](../../aspose.cells/jsonsaveoptions/exporthyperlinktype/) { get; set; } | Representa el tipo de exportación de hipervínculo a json. |
| [ExportNestedStructure](../../aspose.cells/jsonsaveoptions/exportnestedstructure/) { get; set; } | Exportado como estructura Json jerárquica padre-hijo. |
| [ExportStylePool](../../aspose.cells/jsonsaveoptions/exportstylepool/) { get; set; } | Indica si exportar estilos de forma colectiva o individual a cada celda. |
| [HasHeaderRow](../../aspose.cells/jsonsaveoptions/hasheaderrow/) { get; set; } | Indica si el rango contiene una fila de encabezado. |
| [Indent](../../aspose.cells/jsonsaveoptions/indent/) { get; set; } | Indica la sangría. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [Schemas](../../aspose.cells/jsonsaveoptions/schemas/) { get; set; } | El esquema json original de cada hoja de cálculo. |
| [SheetIndexes](../../aspose.cells/jsonsaveoptions/sheetindexes/) { get; set; } | Representa los índices de las hojas exportadas. |
| [SkipEmptyRows](../../aspose.cells/jsonsaveoptions/skipemptyrows/) { get; set; } | Indica si se omiten filas vacías. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ToExcelStruct](../../aspose.cells/jsonsaveoptions/toexcelstruct/) { get; set; } | Indica si se convierte a la estructura json del archivo Excel. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de SmartArt. El valor predeterminado es falso.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. (Hereda de [`SaveOptions`](../saveoptions/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonSaveOptionsDemo
    {
        public static void JsonSaveOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar algunos datos en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Cree una instancia de JsonSaveOptions
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                ExportHyperlinkType = JsonExportHyperlinkType.DisplayString,
                SkipEmptyRows = true,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ExportAsString = true,
                Indent = "  ",
                ExportNestedStructure = false,
                ExportEmptyCells = false,
                AlwaysExportAsJsonObject = false,
                ToExcelStruct = false,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Guarde el libro de trabajo como un archivo JSON
            workbook.Save("JsonSaveOptionsExample.json", saveOptions);

            return;
        }
    }
}
```

### Ver también

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


