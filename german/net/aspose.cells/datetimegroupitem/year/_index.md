---
title: "DateTimeGroupItem.Year"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DateTimeGroupItem-Eigenschaft. Liest und setzt das Jahr des gruppierten Datums/Zeit."
type: docs
url: /de/net/aspose.cells/datetimegroupitem/year/
---
## DateTimeGroupItem.Year property

Liest und setzt das Jahr der gruppierten Datum‑Uhrzeit.

```csharp
public int Year { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyYearDemo
    {
        public static void Run()
        {
            // Ein DateTimeGroupItem nach Jahr gruppiert erstellen
            DateTimeGroupItem dateTimeGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                1,     // Month (ignored when grouping by Year)
                1,     // Day (ignored)
                0,     // Hour (ignored)
                0,     // Minute (ignored)
                0      // Second (ignored)
            );

            // Anfangs-Jahreswert anzeigen
            Console.WriteLine("Initial Year: " + dateTimeGroup.Year);

            // Die Jahres-Eigenschaft ändern
            dateTimeGroup.Year = 2024;

            // Geänderten Jahreswert anzeigen
            Console.WriteLine("Modified Year: " + dateTimeGroup.Year);

            // Demonstrieren, dass andere Eigenschaften bei Gruppierung nach Jahr ignoriert werden
            dateTimeGroup.Month = 12;
            Console.WriteLine("Month value is ignored when grouping by Year: " + dateTimeGroup.Month);
        }
    }
}
```

### Siehe auch

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


