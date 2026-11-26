---
title: "ExportTableOptions.ExportAsString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportTableOptions. Exporta el valor de cadena de las celdas a la DataTable"
type: docs
url: /es/net/aspose.cells/exporttableoptions/exportasstring/
---
## ExportTableOptions.ExportAsString property

Exporta el valor de cadena de las celdas al DataTable.

```csharp
public bool ExportAsString { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra con tipos mixtos
            worksheet.Cells[0, 0].PutValue("ID");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue(123.45);
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue("TextValue");

            // Crear opciones de exportación con ExportAsString establecido en true
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                ExportAsString = true // This forces all values to be exported as strings
            };

            // Exportar datos a DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Mostrar los tipos de datos exportados
            Console.WriteLine("Data exported with ExportAsString=true:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
            }

            // Ahora exportar con ExportAsString=false
            exportOptions.ExportAsString = false;
            DataTable dataTable2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            Console.WriteLine("\nData exported with ExportAsString=false:");
            foreach (DataRow row in dataTable2.Rows)
            {
                Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
            }
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


