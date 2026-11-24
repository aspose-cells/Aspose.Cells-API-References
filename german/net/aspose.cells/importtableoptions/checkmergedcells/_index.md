---
title: "ImportTableOptions.CheckMergedCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions-Eigenschaft. Gibt an, ob zusammengeführte Zellen überprüft werden"
type: docs
url: /de/net/aspose.cells/importtableoptions/checkmergedcells/
---
## ImportTableOptions.CheckMergedCells property

Gibt an, ob zusammengeführte Zellen überprüft werden.

```csharp
public bool CheckMergedCells { get; set; }
```

### Beispiele

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Customer1
    {
        public int CustomerId { get; set; }
        public string Name { get; set; }
    }

    public class ImportTableOptionsPropertyCheckMergedCellsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle zusammengeführte Zellen zur Demonstration
            worksheet.Cells.Merge(3, 3, 2, 1); // Merge D4:D5
            worksheet.Cells[3, 3].PutValue("MergedValue");

            // Erstelle Beispieldaten
            List<Customer1> customers = new List<Customer1>
            {
                new Customer1 { CustomerId = 1, Name = "Customer1" },
                new Customer1 { CustomerId = 2, Name = "Customer2" },
                new Customer1 { CustomerId = 3, Name = "Customer3" }
            };

            // Setze Importoptionen mit aktivierter CheckMergedCells
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = false,
                InsertRows = true,
                CheckMergedCells = true
            };

            // Daten importieren
            worksheet.Cells.ImportCustomObjects(customers, 0, 0, options);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Überprüfe, ob zusammengeführte Zellen erhalten geblieben sind
            Cell mergedCell = worksheet.Cells["D4"];
            Console.WriteLine($"Merged cell value: {mergedCell.StringValue}");
            Console.WriteLine($"Is cell merged: {mergedCell.IsMerged}");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


