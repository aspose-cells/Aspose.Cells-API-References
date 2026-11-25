---
title: "DateTimeGroupItem.Year"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DateTimeGroupItem. Ottiene e imposta l'anno della data e ora raggruppata"
type: docs
url: /it/net/aspose.cells/datetimegroupitem/year/
---
## DateTimeGroupItem.Year property

Ottiene e imposta l'anno della data/ora raggruppata.

```csharp
public int Year { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyYearDemo
    {
        public static void Run()
        {
            // Crea un DateTimeGroupItem raggruppato per Anno
            DateTimeGroupItem dateTimeGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                1,     // Month (ignored when grouping by Year)
                1,     // Day (ignored)
                0,     // Hour (ignored)
                0,     // Minute (ignored)
                0      // Second (ignored)
            );

            // Visualizza il valore iniziale della proprietà Year
            Console.WriteLine("Initial Year: " + dateTimeGroup.Year);

            // Modifica la proprietà Year
            dateTimeGroup.Year = 2024;

            // Visualizza il valore modificato della proprietà Year
            Console.WriteLine("Modified Year: " + dateTimeGroup.Year);

            // Dimostra che le altre proprietà vengono ignorate quando si raggruppa per Year
            dateTimeGroup.Month = 12;
            Console.WriteLine("Month value is ignored when grouping by Year: " + dateTimeGroup.Month);
        }
    }
}
```

### Vedi anche

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


