---
title: "Clase TxtSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.TxtSaveOptions. Representa las opciones de guardado para formato csv/tab delimitado/u otro formato de texto"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/
---
## TxtSaveOptions class

Representa las opciones de guardado para formato csv/tab delimitado/u otro formato de texto.

```csharp
public class TxtSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TxtSaveOptions](txtsaveoptions/#constructor)() | Crea opciones de guardado de archivo de texto. |
| [TxtSaveOptions](txtsaveoptions/#constructor_1)(SaveFormat) | Crea opciones de guardado de archivo de texto. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlwaysQuoted](../../aspose.cells/txtsaveoptions/alwaysquoted/) { get; set; } | (**Obsolete.**) Indica si siempre se agrega '"' para cada campo. Si es verdadero, entonces todos los valores estarán entre comillas; si es falso, los valores solo estarán entre comillas cuando sea necesario (por ejemplo, cuando los valores contengan caracteres especiales como '"' , '\n' o el carácter separador). El valor predeterminado es falso. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena más largo que 32K. Cuando se ingresa un valor más largo que 32K, se truncará.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Dejar el libro de trabajo vacío después de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/txtsaveoptions/encoding/) { get; set; } | Obtiene y establece la codificación predeterminada. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es verdadero.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [ExportAllSheets](../../aspose.cells/txtsaveoptions/exportallsheets/) { get; set; } | Indica si se exportan todas las hojas al archivo de texto. Si es falso, solo se exporta la hoja activa, como en MS Excel. |
| [ExportArea](../../aspose.cells/txtsaveoptions/exportarea/) { get; set; } | El rango de celdas a exportar. |
| [ExportQuotePrefix](../../aspose.cells/txtsaveoptions/exportquoteprefix/) { get; set; } | Indica si el signo de comilla simple debe exportarse como parte del valor de una celda cuando [`QuotePrefix`](../style/quoteprefix/) es verdadero para ella. El valor predeterminado es falso. |
| [FormatStrategy](../../aspose.cells/txtsaveoptions/formatstrategy/) { get; set; } | Obtiene y establece la estrategia de formato al exportar el valor de la celda como cadena. |
| [KeepSeparatorsForBlankRow](../../aspose.cells/txtsaveoptions/keepseparatorsforblankrow/) { get; set; } | Indica si se deben generar separadores para una fila en blanco. El valor predeterminado es falso, por lo que por defecto el contenido de la fila en blanco estará vacío. |
| [LightCellsDataProvider](../../aspose.cells/txtsaveoptions/lightcellsdataprovider/) { get; set; } | El proveedor de datos para guardar el libro de trabajo en modo ligero. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [QuoteType](../../aspose.cells/txtsaveoptions/quotetype/) { get; set; } | Obtiene o establece cómo citar los valores en el archivo de texto exportado. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [Separator](../../aspose.cells/txtsaveoptions/separator/) { get; set; } | Obtiene y establece el carácter delimitador del archivo de texto. |
| [SeparatorString](../../aspose.cells/txtsaveoptions/separatorstring/) { get; set; } | Obtiene y establece un valor de cadena como separador. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Heredado de [`SaveOptions`](../saveoptions/).) |
| [TrimLeadingBlankRowAndColumn](../../aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/) { get; set; } | Indica si las filas y columnas en blanco iniciales deben recortarse como lo hace MS Excel. El valor predeterminado es verdadero. |
| [TrimTailingBlankCells](../../aspose.cells/txtsaveoptions/trimtailingblankcells/) { get; set; } | Indica si las celdas en blanco finales en una fila deben recortarse. El valor predeterminado es falso. |
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

    public class TxtSaveOptionsDemo
    {
        public static void TxtSaveOptionsExample()
        {
            // Crear un libro de trabajo con algunos datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Smith");
            worksheet.Cells["B3"].PutValue(25);

            // Crear un objeto TxtSaveOptions y establecer propiedades
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                SeparatorString = ",",
                Encoding = Encoding.UTF8,
                AlwaysQuoted = false,
                QuoteType = TxtValueQuoteType.Normal,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                TrimLeadingBlankRowAndColumn = true,
                TrimTailingBlankCells = false,
                KeepSeparatorsForBlankRow = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                ExportQuotePrefix = false,
                ExportAllSheets = false,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Guarde el libro de trabajo como un archivo de texto con las opciones especificadas
            workbook.Save("TxtSaveOptionsExample.txt", saveOptions);

            Console.WriteLine("Workbook saved successfully with TxtSaveOptions.");
        }
    }
}
```

### Ver también

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


