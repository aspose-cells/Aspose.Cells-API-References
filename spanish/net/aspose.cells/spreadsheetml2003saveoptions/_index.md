---
title: "Clase SpreadsheetML2003SaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.SpreadsheetML2003SaveOptions. Representa las opciones para guardar un archivo spreadml de Excel 2003"
type: docs
url: /es/net/aspose.cells/spreadsheetml2003saveoptions/
---
## SpreadsheetML2003SaveOptions class

Representa las opciones para guardar el archivo Excel 2003 spreadml.

```csharp
public class SpreadsheetML2003SaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SpreadsheetML2003SaveOptions](spreadsheetml2003saveoptions/#constructor)() | Crea las opciones para guardar un archivo spreadml de Excel 2003. |
| [SpreadsheetML2003SaveOptions](spreadsheetml2003saveoptions/#constructor_1)(SaveFormat) | (**Obsoleto.**) Crea las opciones para guardar un archivo spreadml de Excel 2003. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando se ingresa un valor más largo que 32K, se truncará.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dejar el libro de trabajo vacío después de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ExportColumnIndexOfCell](../../aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/) { get; set; } | El valor predeterminado es false, lo que significa que el índice de columna se ignorará si la celda es contigua a la celda anterior. |
| [IsIndentedFormatting](../../aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/) { get; set; } | Hace que los elementos secundarios se sangren. |
| [LimitAsXls](../../aspose.cells/spreadsheetml2003saveoptions/limitasxls/) { get; set; } | Límite como xls, el índice máximo de fila es 65535 y el índice máximo de columna es 255. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de SmartArt. El valor predeterminado es falso.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia. (Hereda de [`SaveOptions`](../saveoptions/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SpreadsheetML2003SaveOptionsDemo
    {
        public static void SpreadsheetML2003SaveOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar algunos datos en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);

            // Crear una instancia de SpreadsheetML2003SaveOptions
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();

            // Establecer propiedades
            saveOptions.IsIndentedFormatting = true;
            saveOptions.LimitAsXls = false;
            saveOptions.ExportColumnIndexOfCell = true;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = @"C:\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Guarde el libro de trabajo con las opciones de guardado especificadas
            workbook.Save("SpreadsheetML2003Example.xml", saveOptions);

            return;
        }
    }
}
```

### Ver también

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


