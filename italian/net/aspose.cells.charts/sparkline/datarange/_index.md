---
title: "Sparkline.DataRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Sparkline. Rappresenta l'intervallo di dati della sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparkline/datarange/
---
## Sparkline.DataRange property

Rappresenta l'intervallo di dati dello sparkline.

```csharp
public string DataRange { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyDataRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(7);
            sheet.Cells["A4"].PutValue(2);
            sheet.Cells["A5"].PutValue(9);

            // Aggiungi un gruppo sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A5", false, new CellArea { StartRow = 0, StartColumn = 1, EndRow = 0, EndColumn = 1 });
            SparklineGroup group = sheet.SparklineGroups[idx];
            
            // Accedi alla prima sparkline e visualizza il suo intervallo di dati
            Sparkline sparkline = group.Sparklines[0];
            Console.WriteLine("Sparkline DataRange: " + sparkline.DataRange);
        }
    }
}
```

### Vedi anche

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


