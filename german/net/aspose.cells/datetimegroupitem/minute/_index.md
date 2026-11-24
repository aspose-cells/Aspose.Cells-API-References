---
title: "DateTimeGroupItem.Minute"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DateTimeGroupItem-Eigenschaft. Gibt die Minute des gruppierten Datums/Uhrzeit zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/datetimegroupitem/minute/
---
## DateTimeGroupItem.Minute property

Liest und setzt die Minute der gruppierten Datum‑Uhrzeit.

```csharp
public int Minute { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinuteDemo
    {
        public static void Run()
        {
            // Ein DateTimeGroupItem mit Anfangswerten erstellen
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                10,
                5,
                14,
                30,
                45
            );

            // Anfänglichen Minutenwert anzeigen
            Console.WriteLine("Initial Minute: " + dateTimeGroupItem.Minute);

            // Minutenwert ändern
            dateTimeGroupItem.Minute = 15;

            // Modifizierten Minutenwert anzeigen
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);

            // Ein neues DateTimeGroupItem nur mit Minuten-Gruppierung erstellen
            DateTimeGroupItem minuteGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Minute,
                0, 0, 0, 0, 45, 0
            );

            // Minute aus der Minuten-Gruppierung anzeigen
            Console.WriteLine("Minute from Minute Grouping: " + minuteGroup.Minute);
        }
    }
}
```

### Siehe auch

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


