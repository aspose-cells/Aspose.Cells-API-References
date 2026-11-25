---
title: "DateTimeGroupItem.Hour"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DateTimeGroupItem. Ottiene e imposta l'ora del data/ora raggruppato"
type: docs
url: /it/net/aspose.cells/datetimegroupitem/hour/
---
## DateTimeGroupItem.Hour property

Ottiene e imposta l'ora della data/ora raggruppata.

```csharp
public int Hour { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyHourDemo
    {
        public static void Run()
        {
            // Crea un DateTimeGroupItem con raggruppamento per ora
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Hour,
                2023,  // Year
                10,     // Month
                5,      // Day
                14,     // Hour
                0,      // Minute
                0      // Second
            );

            // Visualizza il valore iniziale dell'ora
            Console.WriteLine("Initial Hour: " + dateTimeGroupItem.Hour);

            // Modifica la proprietà hour
            dateTimeGroupItem.Hour = 18;

            // Visualizza il valore hour modificato
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
        }
    }
}
```

### Vedi anche

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


