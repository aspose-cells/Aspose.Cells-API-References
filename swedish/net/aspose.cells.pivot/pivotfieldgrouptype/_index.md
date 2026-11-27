---
title: "Enum PivotFieldGroupType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotFieldGroupType enum. Representerar grupptypen för pivottfältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldgrouptype/
---
## PivotFieldGroupType enumeration

Representerar grupptypen för pivottfältet.

```csharp
public enum PivotFieldGroupType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen grupp |
| DateTimeRange | `1` | Grupperad efter DateTime-intervall. |
| NumbericRange | `2` | Grupperad efter numeriskt intervall. |
| NumericRange | `2` | Grupperad efter numeriskt intervall. |
| Discrete | `3` | Grupperad efter diskreta punkter. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotFieldGroupTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Date");
            Style style = workbook.CreateStyle();
            style.Number = 14; // m/d/yyyy format
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].SetStyle(style);
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].SetStyle(style);
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A4"].SetStyle(style);

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value field

            // Gruppera datumfältet
            PivotField dateField = pivotTable.RowFields[0];
            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // Åtkomst och visa gruppinställningar
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            Console.WriteLine("Group Type: " + groupSettings.Type);
            Console.WriteLine("Interval: " + groupSettings.Interval);
            Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // Spara arbetsboken
            workbook.Save("PivotFieldGroupTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


