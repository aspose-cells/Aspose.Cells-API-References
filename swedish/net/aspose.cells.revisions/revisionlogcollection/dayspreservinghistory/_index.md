---
title: "RevisionLogCollection.DaysPreservingHistory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionLogCollection egenskap. Hämtar och anger antalet dagar som kalkylprogrammet kommer att behålla förändringshistoriken för den här arbetsboken"
type: docs
url: /sv/net/aspose.cells.revisions/revisionlogcollection/dayspreservinghistory/
---
## RevisionLogCollection.DaysPreservingHistory property

Hämtar och anger antalet dagar som kalkylprogrammet kommer att behålla ändringshistoriken för den här arbetsboken.

```csharp
public int DaysPreservingHistory { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionPropertyDaysPreservingHistoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Value");
            
            // Ställ in egenskapen DaysPreservingHistory
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 40;
            
            string outputPath = "output_DaysPreservingHistory.xlsx";
            workbook.Save(outputPath);
            
            // Läs in igen för att verifiera egenskapen
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("DaysPreservingHistory: " + 
                loadedWorkbook.Worksheets.RevisionLogs.DaysPreservingHistory);
        }
    }
}
```

### Se även

* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


