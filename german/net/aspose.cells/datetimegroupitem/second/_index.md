---
title: "DateTimeGroupItem.Second"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DateTimeGroupItem-Eigenschaft. Gibt die Sekunde des gruppierten Datums zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/datetimegroupitem/second/
---
## DateTimeGroupItem.Second property

Liest und setzt die Sekunde der gruppierten Datum‑Uhrzeit.

```csharp
public int Second { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertySecondDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                        // Month
                5,                         // Day
                14,                        // Hour
                30,                        // Minute
                45                         // Second
            );

            // Anfangssekundenwert anzeigen
            Console.WriteLine("Initial Second: " + dateTimeGroupItem.Second);

            // Sekundenwert ändern
            dateTimeGroupItem.Second = 50;
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);

            // Eine weitere Instanz mit anderem Sekundenwert erstellen
            DateTimeGroupItem anotherItem = new DateTimeGroupItem(
                DateTimeGroupingType.Day,
                2023,
                10,
                5,
                14,
                30,
                0  // Second set to 0
            );
            Console.WriteLine("Another Item Second: " + anotherItem.Second);
        }
    }
}
```

### Siehe auch

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


