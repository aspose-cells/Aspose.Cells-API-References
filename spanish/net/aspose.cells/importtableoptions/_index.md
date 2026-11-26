---
title: "Clase ImportTableOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ImportTableOptions. Representa las opciones de importación de datos en celdas"
type: docs
url: /es/net/aspose.cells/importtableoptions/
---
## ImportTableOptions class

Representa las opciones de importación de datos en celdas.

```csharp
public class ImportTableOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ImportTableOptions](importtableoptions/)() | Crea las opciones de importación predeterminadas. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CheckMergedCells](../../aspose.cells/importtableoptions/checkmergedcells/) { get; set; } | Indica si se deben comprobar celdas combinadas. |
| [ColumnIndexes](../../aspose.cells/importtableoptions/columnindexes/) { get; set; } | Obtiene o establece las columnas (basadas en 0) a importar del origen de datos. null significa que se deben importar todas las columnas. |
| [ConvertGridStyle](../../aspose.cells/importtableoptions/convertgridstyle/) { get; set; } | Indica si se debe aplicar el estilo de la vista de cuadrícula a las celdas. |
| [ConvertNumericData](../../aspose.cells/importtableoptions/convertnumericdata/) { get; set; } | Obtiene o establece un valor que indica si el valor de cadena debe convertirse a numérico o a fecha. |
| [DateFormat](../../aspose.cells/importtableoptions/dateformat/) { get; set; } | Obtiene o establece la cadena de formato de fecha para celdas con valores de fecha y hora importados. |
| [DefaultValues](../../aspose.cells/importtableoptions/defaultvalues/) { get; set; } | El valor predeterminado para el valor en la tabla es null. |
| [ExportCaptionAsFieldName](../../aspose.cells/importtableoptions/exportcaptionasfieldname/) { get; set; } | Indica si se exporta el título como nombre de campo |
| [InsertRows](../../aspose.cells/importtableoptions/insertrows/) { get; set; } | Indica si se deben agregar filas nuevas al importar registros de datos. |
| [IsFieldNameShown](../../aspose.cells/importtableoptions/isfieldnameshown/) { get; set; } | Indica si se debe importar el nombre del campo. |
| [IsFormulas](../../aspose.cells/importtableoptions/isformulas/) { get; set; } | Indica si los datos son fórmulas. |
| [IsHtmlString](../../aspose.cells/importtableoptions/ishtmlstring/) { get; set; } | Indica si el valor contiene etiquetas HTML. |
| [NumberFormats](../../aspose.cells/importtableoptions/numberformats/) { get; set; } | Obtiene o establece los formatos numéricos |
| [ShiftFirstRowDown](../../aspose.cells/importtableoptions/shiftfirstrowdown/) { get; set; } | Indica si se desplaza la primera fila hacia abajo al insertar filas. |
| [Styles](../../aspose.cells/importtableoptions/styles/) { get; set; } | Obtiene y establece los estilos para cada columna de la tabla. |
| [TotalColumns](../../aspose.cells/importtableoptions/totalcolumns/) { get; set; } | Obtiene o establece el recuento total de columnas a importar del origen de datos. -1 significa todas las filas del origen de datos dado. |
| [TotalRows](../../aspose.cells/importtableoptions/totalrows/) { get; set; } | Obtiene o establece el recuento total de filas a importar del origen de datos. -1 significa todas las filas del origen de datos dado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsDemo
    {
        public static void ImportTableOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un DataTable para importar
            DataTable dataTable = new DataTable("SampleData");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Date", typeof(DateTime));
            dataTable.Rows.Add(1, "John Doe", DateTime.Now);
            dataTable.Rows.Add(2, "Jane Smith", DateTime.Now.AddDays(1));

            // Crear una instancia de ImportTableOptions
            ImportTableOptions importOptions = new ImportTableOptions
            {
                ConvertGridStyle = true,
                ConvertNumericData = true,
                InsertRows = true,
                ShiftFirstRowDown = false,
                IsFieldNameShown = true,
                ExportCaptionAsFieldName = false,
                DateFormat = "yyyy-MM-dd",
                TotalRows = -1, // Import all rows
                TotalColumns = -1, // Import all columns
                IsHtmlString = false,
                CheckMergedCells = false
            };

            // Importar la DataTable en la hoja de cálculo
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Guarda el libro de trabajo
            workbook.Save("ImportTableOptionsExample.xlsx");
            workbook.Save("ImportTableOptionsExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


