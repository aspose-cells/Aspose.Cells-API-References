---
title: "Worksheet.Timelines"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Holen Sie die Timeline‑Sammlung im Arbeitsblatt"
type: docs
url: /de/net/aspose.cells/worksheet/timelines/
---
## Worksheet.Timelines property

Rufen Sie die Timeline‑Sammlung im Arbeitsblatt ab.

```csharp
public TimelineCollection Timelines { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            sheet.Cells["A1"].Value = "Ship Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 1, 15);
            sheet.Cells["A4"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Ship Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Timeline‑Steuerelement für die Pivot‑Tabelle hinzufügen
            sheet.Timelines.Add(pivotTable, 0, 0, "Ship Date");

            // Speichere die Arbeitsmappe
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TimelineCollection](../../../aspose.cells.timelines/timelinecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


