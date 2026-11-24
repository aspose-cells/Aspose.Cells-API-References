---
title: "DateTimeGroupItem.Hour"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DateTimeGroupItem-Eigenschaft. Liest und setzt die Stunde des gruppierten Datums/Zeit."
type: docs
url: /de/net/aspose.cells/datetimegroupitem/hour/
---
## DateTimeGroupItem.Hour property

Liest und setzt die Stunde der gruppierten Datum‑Uhrzeit.

```csharp
public int Hour { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyHourDemo
    {
        public static void Run()
        {
            // Ein DateTimeGroupItem mit Stunden-Gruppierung erstellen
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Hour,
                2023,  // Year
                10,     // Month
                5,      // Day
                14,     // Hour
                0,      // Minute
                0      // Second
            );

            // Anfangs-Stundenwert anzeigen
            Console.WriteLine("Initial Hour: " + dateTimeGroupItem.Hour);

            // Die Stundeneigenschaft ändern
            dateTimeGroupItem.Hour = 18;

            // Geänderten Stundenwert anzeigen
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
        }
    }
}
```

### Siehe auch

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


