---
title: "DateTimeGroupItem.Month"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "DateTimeGroupItem proprietà. Ottiene e imposta il mese della data e ora raggruppata"
type: docs
url: /it/net/aspose.cells/datetimegroupitem/month/
---
## DateTimeGroupItem.Month property

Ottiene e imposta il mese della data/ora raggruppata.

```csharp
public int Month { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMonthDemo
    {
        public static void Run()
        {
            // Crea un DateTimeGroupItem raggruppato per Month
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Month,
                2023,
                10,
                1,
                0,
                0,
                0
            );

            // Visualizza il valore iniziale del mese
            Console.WriteLine("Initial Month: " + dateTimeGroupItem.Month);

            // Modifica il valore del mese
            dateTimeGroupItem.Month = 12;
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);

            // Crea un altro DateTimeGroupItem con raggruppamento diverso
            DateTimeGroupItem yearlyItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                1,
                1,
                0,
                0,
                0
            );

            // Mostra che la proprietà Month è ancora accessibile anche quando è raggruppato per Year
            Console.WriteLine("Yearly Grouping - Month: " + yearlyItem.Month);
        }
    }
}
```

### Vedi anche

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


