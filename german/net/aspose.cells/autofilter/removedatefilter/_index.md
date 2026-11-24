---
title: "AutoFilter.RemoveDateFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Entfernt einen Datumsfilter"
type: docs
url: /de/net/aspose.cells/autofilter/removedatefilter/
---
## AutoFilter.RemoveDateFilter method

Entfernt einen Datumsfilter.

```csharp
public void RemoveDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | Int32 | Der ganzzahlige Versatz des Feldes, auf dem der Filter basieren soll (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| dateTimeGroupingType | DateTimeGroupingType | Der Gruppierungstyp |
| Jahr | Int32 | Das Jahr. |
| Monat | Int32 | Der Monat. |
| Tag | Int32 | Der Tag. |
| Stunde | Int32 | Die Stunde. |
| Minute | Int32 | Die Minute. |
| Sekunde | Int32 | Die Sekunde. |

### Hinweise

Wenn DateTimeGroupingType Year ist, wirkt nur das Parameter year. Wenn DateTiemGroupingType Month ist, wirken nur die Parameter year und month.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveDateFilterWithInt32DateTimeGroupingTypeInt32Demo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Beispieldaten mit Datumsangaben hinzufügen
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue(new DateTime(2020, 1, 7));
            sheet.Cells["A3"].PutValue(new DateTime(2020, 1, 8));
            sheet.Cells["A4"].PutValue(new DateTime(2020, 1, 9));
            
            // Auto-Filter anwenden
            sheet.AutoFilter.Range = "A1:A4";
            
            // Datumsfilter für Tag 7 hinzufügen
            sheet.AutoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Überprüfen, dass der Filter angewendet wurde
            Console.WriteLine("Row 2 hidden: " + sheet.Cells.IsRowHidden(1)); // Should be true
            
            // Den Datumsfilter entfernen
            sheet.AutoFilter.RemoveDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Überprüfen, dass der Filter entfernt wurde
            Console.WriteLine("Row 2 hidden after removal: " + sheet.Cells.IsRowHidden(1)); // Should be false
        }
    }
}
```

### Siehe auch

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


