---
title: "DateTimeGroupItem.Second"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DateTimeGroupItem. Ottiene e imposta il secondo della data/ora raggruppata"
type: docs
url: /it/net/aspose.cells/datetimegroupitem/second/
---
## DateTimeGroupItem.Second property

Ottiene e imposta il secondo della data/ora raggruppata.

```csharp
public int Second { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertySecondDemo
    {
        public static void Run()
        {
            // Crea un'istanza di DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                        // Month
                5,                         // Day
                14,                        // Hour
                30,                        // Minute
                45                         // Second
            );

            // Visualizza il valore iniziale del secondo
            Console.WriteLine("Initial Second: " + dateTimeGroupItem.Second);

            // Modifica il valore del secondo
            dateTimeGroupItem.Second = 50;
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);

            // Crea un'altra istanza con un valore del secondo diverso
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

### Vedi anche

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


