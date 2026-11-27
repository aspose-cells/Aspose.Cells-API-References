---
title: "Worksheet.Timelines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämta Timeline-samlingen i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/timelines/
---
## Worksheet.Timelines property

Hämta Timeline-samlingen i arbetsbladet

```csharp
public TimelineCollection Timelines { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTimelinesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].Value = "Ship Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 1, 15);
            sheet.Cells["A4"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Ship Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Lägg till tidslinjekontroll för pivottabellen
            sheet.Timelines.Add(pivotTable, 0, 0, "Ship Date");

            // Spara arbetsboken
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Se även

* class [TimelineCollection](../../../aspose.cells.timelines/timelinecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


