---
title: "DateTimeGroupItem.MinValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DateTimeGroupItem. Ottiene il valore minimo"
type: docs
url: /it/net/aspose.cells/datetimegroupitem/minvalue/
---
## DateTimeGroupItem.MinValue property

Ottiene il valore minimo.

```csharp
public DateTime MinValue { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinValueDemo
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

            // Dimostra la proprietà MinValue
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);

            // Mostra altre proprietà per contesto
            Console.WriteLine("Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Date Components: {0}-{1}-{2} {3}:{4}:{5}",
                dateTimeGroupItem.Year,
                dateTimeGroupItem.Month,
                dateTimeGroupItem.Day,
                dateTimeGroupItem.Hour,
                dateTimeGroupItem.Minute,
                dateTimeGroupItem.Second);
        }
    }
}
```

### Vedi anche

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


