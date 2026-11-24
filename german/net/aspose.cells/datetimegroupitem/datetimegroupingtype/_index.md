---
title: "DateTimeGroupItem.DateTimeGroupingType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DateTimeGroupItem-Eigenschaft. Gibt den Gruppentyp zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/datetimegroupitem/datetimegroupingtype/
---
## DateTimeGroupItem.DateTimeGroupingType property

Liest und setzt den Gruppentyp.

```csharp
public DateTimeGroupingType DateTimeGroupingType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDateTimeGroupingTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                       // Month
                5,                         // Day
                14,                       // Hour
                30,                       // Minute
                45                        // Second
            );

            // Anfängliche Eigenschaften anzeigen
            Console.WriteLine("Initial Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine($"Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}-{dateTimeGroupItem.Day}");

            // Gruppierungstyp und Datumskomponenten ändern
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;

            // Geänderte Eigenschaften anzeigen
            Console.WriteLine("Modified Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine($"Modified Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}");
        }
    }
}
```

### Siehe auch

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


