---
title: "PivotDateTimeRangeGroupSettings.IsGroupedBy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotDateTimeRangeGroupSettings‑metod. Kontrollerar om fältet är grupperat efter typen"
type: docs
url: /sv/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/isgroupedby/
---
## PivotDateTimeRangeGroupSettings.IsGroupedBy method

Kontrollera om fältet är grupperat efter typen.

```csharp
public bool IsGroupedBy(PivotGroupByType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | PivotGroupByType | Grupptypen |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsMethodIsGroupedByWithPivotGroupByTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Gruppera efter datum
            PivotField dateField = pivotTable.RowFields[0];
            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);

            // Kontrollera gruppering
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            bool isGroupedByMonths = groupSettings.IsGroupedBy(PivotGroupByType.Months);
            
            Console.WriteLine($"Is grouped by months: {isGroupedByMonths}");
        }
    }
}
```

### Se även

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


