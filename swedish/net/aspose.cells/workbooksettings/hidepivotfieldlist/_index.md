---
title: "WorkbookSettings.HidePivotFieldList"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Hämtar och anger om fältlistan för pivottabellen ska döljas"
type: docs
url: /sv/net/aspose.cells/workbooksettings/hidepivotfieldlist/
---
## WorkbookSettings.HidePivotFieldList property

Hämtar och anger om fältlistan för pivottabellen ska döljas.

```csharp
public bool HidePivotFieldList { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyHidePivotFieldListDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("A");
            sheet.Cells["B4"].PutValue(150);

            // Skapa pivottabell
            int index = workbook.Worksheets.Add(SheetType.Worksheet);
            Worksheet pivotSheet = workbook.Worksheets[index];
            pivotSheet.Name = "PivotTable";
            
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:B4", "C3");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Åtkomst till arbetsboksinställningar och sätt HidePivotFieldList-egenskapen
            WorkbookSettings settings = workbook.Settings;
            settings.HidePivotFieldList = true; // Hide the pivot field list

            // Spara arbetsboken
            workbook.Save("HidePivotFieldListDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


