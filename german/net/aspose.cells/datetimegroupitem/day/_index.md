---
title: "DateTimeGroupItem.Day"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DateTimeGroupItem-Eigenschaft. Gibt den Tag des gruppierten Datums/Uhrzeit zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/datetimegroupitem/day/
---
## DateTimeGroupItem.Day property

Liest und setzt den Tag der gruppierten Datum‑Uhrzeit.

```csharp
public int Day { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDayDemo
    {
        public static void Run()
        {
            // Ein DateTimeGroupItem nach Jahr gruppiert erstellen
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                10,    // Month
                5,     // Day
                14,    // Hour
                30,    // Minute
                45     // Second
            );

            // Anfänglichen Tageswert anzeigen
            Console.WriteLine("Initial Day: " + dateTimeGroupItem.Day);

            // Tag-Eigenschaft ändern
            dateTimeGroupItem.Day = 25;
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);

            // Ein weiteres DateTimeGroupItem, gruppiert nach Tag, erstellen, um die Bedeutung der Day-Eigenschaft zu demonstrieren
            DateTimeGroupItem dayGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Day,
                2023,
                10,
                15,  // Initial day
                0,
                0,
                0
            );

            Console.WriteLine("\nDay-grouped item initial Day: " + dayGroupItem.Day);
            dayGroupItem.Day = 20;
            Console.WriteLine("Day-grouped item modified Day: " + dayGroupItem.Day);
        }
    }
}
```

### Siehe auch

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


