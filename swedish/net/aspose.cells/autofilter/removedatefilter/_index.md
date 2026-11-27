---
title: "AutoFilter.RemoveDateFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Tar bort ett datumfilter"
type: docs
url: /sv/net/aspose.cells/autofilter/removedatefilter/
---
## AutoFilter.RemoveDateFilter method

Tar bort ett datumfilter.

```csharp
public void RemoveDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| dateTimeGroupingType | DateTimeGroupingType | Grupperingstypen |
| år | Int32 | Året. |
| månad | Int32 | Månaden. |
| dag | Int32 | Dagen. |
| timme | Int32 | Timmen. |
| minut | Int32 | Minuten. |
| sekund | Int32 | Sekunden. |

### Anmärkningar

Om DateTimeGroupingType är Year, påverkar bara parametern year. Om DateTiemGroupingType är Month, påverkar bara parametrarna year och month.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveDateFilterWithInt32DateTimeGroupingTypeInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata med datum
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue(new DateTime(2020, 1, 7));
            sheet.Cells["A3"].PutValue(new DateTime(2020, 1, 8));
            sheet.Cells["A4"].PutValue(new DateTime(2020, 1, 9));
            
            // Applicera autofilter
            sheet.AutoFilter.Range = "A1:A4";
            
            // Lägg till datumfilter för dag 7
            sheet.AutoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Verifiera att filtret har tillämpats
            Console.WriteLine("Row 2 hidden: " + sheet.Cells.IsRowHidden(1)); // Should be true
            
            // Ta bort datumfiltret
            sheet.AutoFilter.RemoveDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Verifiera att filtret har tagits bort
            Console.WriteLine("Row 2 hidden after removal: " + sheet.Cells.IsRowHidden(1)); // Should be false
        }
    }
}
```

### Se även

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


