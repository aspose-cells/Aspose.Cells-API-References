---
title: "Enum PivotGroupByType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotGroupByType enum. Representerar grupperingstyp"
type: docs
url: /sv/net/aspose.cells.pivot/pivotgroupbytype/
---
## PivotGroupByType enumeration

Representerar gruppera‑efter‑typ.

```csharp
[Flags]
public enum PivotGroupByType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| RangeOfValues | `1` | Gruppera efter siffror. |
| Numbers | `1` | Gruppera efter siffror. |
| Seconds | `2` | Visar sekunder-grupperingstyp. |
| Minutes | `4` | Visar minuter-grupperingstyp. |
| Hours | `8` | Visar timmar-grupperingstyp. |
| Days | `10` | Visar dagar-grupperingstyp. |
| Months | `20` | Visar månader-grupperingstyp. |
| Quarters | `40` | Visar kvartal-grupperingstyp. |
| Years | `80` | Visar år-grupperingstyp. |
| DateTimes | `FE` | Visar alla grupperings typer för datum och tid. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGroupByTypeDemo
    {
        public static void PivotGroupByTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Date");
            Style style = workbook.CreateStyle();
            style.Number = 14;//m/d/yyy
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

            //TODO
            PivotField dateField = pivotTable.RowFields[0];

            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // Kom åt gruppinställningarna
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

            // Skriv ut gruppinställningarna
            Console.WriteLine("Group Type: " + groupSettings.Type);
            Console.WriteLine("Start Date: " + groupSettings.Start);
            Console.WriteLine("End Date: " + groupSettings.End);
            Console.WriteLine("Interval: " + groupSettings.Interval);
            Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // Spara arbetsboken
            workbook.Save("PivotGroupByTypeExample.xlsx");
            
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


