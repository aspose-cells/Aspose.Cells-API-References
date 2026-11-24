---
title: "ICellsDataTable.Columns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ICellsDataTable-Eigenschaft. Gibt den Spaltennamen zurück"
type: docs
url: /de/net/aspose.cells/icellsdatatable/columns/
---
## ICellsDataTable.Columns property

Liest den Namen der Spalten.

```csharp
public string[] Columns { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyColumnsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Beispieldaten
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["C1"].PutValue("Stock");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["C2"].PutValue(15);

            try
            {
                // Datenbereich in ICellsDataTable exportieren
                ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 2, 3);

                // Spaltennamen anzeigen
                Console.WriteLine("Column names in the data table:");
                foreach (string column in dataTable.Columns)
                {
                    Console.WriteLine(column);
                }

                // Anzahl der Spalten anzeigen
                Console.WriteLine($"Total columns: {dataTable.Columns.Length}");

                // Speichere die Arbeitsmappe
                workbook.Save("ColumnsDemo.xlsx");
                Console.WriteLine("Columns property demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


