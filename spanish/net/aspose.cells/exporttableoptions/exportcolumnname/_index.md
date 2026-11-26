---
title: "ExportTableOptions.ExportColumnName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportTableOptions. Indica si los datos en la primera fila se exportan al nombre de columna del DataTable. El valor predeterminado es false."
type: docs
url: /es/net/aspose.cells/exporttableoptions/exportcolumnname/
---
## ExportTableOptions.ExportColumnName property

Indica si los datos de la primera fila se exportan al nombre de columna del DataTable. El valor predeterminado es false.

```csharp
public bool ExportColumnName { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportColumnNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear datos de muestra en la hoja de cálculo
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Data1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Data2");

            // Configurar opciones de exportación
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true; // Demonstrating ExportColumnName property
            options.IsVertical = true;
            options.Indexes = new int[] { 0, 1 }; // Export all columns

            // Exportar datos de la hoja de cálculo al DataTable
            DataTable dataTable = cells.ExportDataTable(0, 0, 4, 2, options);

            // Muestre los datos exportados
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Column1"]}, {row["Column2"]}");
            }
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


