---
title: "DateTimeGroupItem.Month"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DateTimeGroupItem-Eigenschaft. Gibt den Monat des gruppierten Datums zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/datetimegroupitem/month/
---
## DateTimeGroupItem.Month property

Liest und setzt den Monat der gruppierten Datum‑Uhrzeit.

```csharp
public int Month { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMonthDemo
    {
        public static void Run()
        {
            // Ein DateTimeGroupItem nach Monat gruppiert erstellen
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Month,
                2023,
                10,
                1,
                0,
                0,
                0
            );

            // Anfangsmonatwert anzeigen
            Console.WriteLine("Initial Month: " + dateTimeGroupItem.Month);

            // Monatswert ändern
            dateTimeGroupItem.Month = 12;
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);

            // Ein weiteres DateTimeGroupItem mit anderer Gruppierung erstellen
            DateTimeGroupItem yearlyItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                1,
                1,
                0,
                0,
                0
            );

            // Zeigen, dass die Month-Eigenschaft weiterhin zugänglich ist, selbst wenn nach Jahr gruppiert wird
            Console.WriteLine("Yearly Grouping - Month: " + yearlyItem.Month);
        }
    }
}
```

### Siehe auch

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


