---
title: "ImportTableOptions.CheckMergedCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions-egenskap. Anger om sammanslagna celler ska kontrolleras"
type: docs
url: /sv/net/aspose.cells/importtableoptions/checkmergedcells/
---
## ImportTableOptions.CheckMergedCells property

Anger om sammanslagna celler ska kontrolleras.

```csharp
public bool CheckMergedCells { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa sammanslagna celler för demonstration
            worksheet.Cells.Merge(3, 3, 2, 1); // Merge D4:D5
            worksheet.Cells[3, 3].PutValue("MergedValue");

            // Skapa exempeldata
            List<Customer1> customers = new List<Customer1>
            {
                new Customer1 { CustomerId = 1, Name = "Customer1" },
                new Customer1 { CustomerId = 2, Name = "Customer2" },
                new Customer1 { CustomerId = 3, Name = "Customer3" }
            };

            // Ställ in importalternativ med CheckMergedCells aktiverat
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = false,
                InsertRows = true,
                CheckMergedCells = true
            };

            // Importera data
            worksheet.Cells.ImportCustomObjects(customers, 0, 0, options);

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Verifiera att sammanslagna celler bevarades
            Cell mergedCell = worksheet.Cells["D4"];
            Console.WriteLine($"Merged cell value: {mergedCell.StringValue}");
            Console.WriteLine($"Is cell merged: {mergedCell.IsMerged}");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


