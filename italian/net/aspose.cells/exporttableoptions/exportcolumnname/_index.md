---
title: "ExportTableOptions.ExportColumnName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ExportTableOptions proprietà. Indica se i dati nella prima riga vengono esportati nel nome colonna del DataTable. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/exporttableoptions/exportcolumnname/
---
## ExportTableOptions.ExportColumnName property

Indica se i dati nella prima riga vengono esportati nel nome della colonna della DataTable. Il valore predefinito è false.

```csharp
public bool ExportColumnName { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea dati di esempio nel foglio di lavoro
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Data1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Data2");

            // Configura le opzioni di esportazione
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true; // Demonstrating ExportColumnName property
            options.IsVertical = true;
            options.Indexes = new int[] { 0, 1 }; // Export all columns

            // Esporta dati dal foglio di lavoro al DataTable
            DataTable dataTable = cells.ExportDataTable(0, 0, 4, 2, options);

            // Visualizza i dati esportati
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Column1"]}, {row["Column2"]}");
            }
        }
    }
}
```

### Vedi anche

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


