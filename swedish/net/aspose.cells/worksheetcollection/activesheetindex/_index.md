---
title: "WorksheetCollection.ActiveSheetIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Representerar indexet för det aktiva bladet när kalkylbladet öppnas"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/activesheetindex/
---
## WorksheetCollection.ActiveSheetIndex property

Representerar indexet för det aktiva kalkylbladet när kalkylarket öppnas.

```csharp
public int ActiveSheetIndex { get; set; }
```

### Anmärkningar

Bladindex är nollbaserat.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med 3 blad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Ställ in det aktiva bladindexet till 1 (andra bladet)
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Verifiera det aktiva bladet
            Console.WriteLine("Active Sheet: " + workbook.Worksheets[workbook.Worksheets.ActiveSheetIndex].Name);

            // Spara arbetsboken
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ActiveSheetDemo.xlsx");
            workbook.Save(outputPath);

            Console.WriteLine("File saved to: " + outputPath);
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


