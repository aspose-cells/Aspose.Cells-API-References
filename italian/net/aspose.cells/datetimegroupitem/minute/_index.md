---
title: "DateTimeGroupItem.Minute"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "DateTimeGroupItem proprietà. Ottiene e imposta il minuto della data e ora raggruppata"
type: docs
url: /it/net/aspose.cells/datetimegroupitem/minute/
---
## DateTimeGroupItem.Minute property

Ottiene e imposta il minuto della data/ora raggruppata.

```csharp
public int Minute { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinuteDemo
    {
        public static void Run()
        {
            // Crea un DateTimeGroupItem con valori iniziali
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                10,
                5,
                14,
                30,
                45
            );

            // Visualizza il valore iniziale del minuto
            Console.WriteLine("Initial Minute: " + dateTimeGroupItem.Minute);

            // Modifica il valore del minuto
            dateTimeGroupItem.Minute = 15;

            // Visualizza il valore del minuto modificato
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);

            // Crea un nuovo DateTimeGroupItem con raggruppamento solo per minuto
            DateTimeGroupItem minuteGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Minute,
                0, 0, 0, 0, 45, 0
            );

            // Visualizza il minuto dal raggruppamento per minuto
            Console.WriteLine("Minute from Minute Grouping: " + minuteGroup.Minute);
        }
    }
}
```

### Vedi anche

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


