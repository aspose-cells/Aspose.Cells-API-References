---
title: "Classe DateTimeGroupItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DateTimeGroupItem. Rappresenta l'impostazione del gruppo di data/ora"
type: docs
url: /it/net/aspose.cells/datetimegroupitem/
---
## DateTimeGroupItem class

Rappresenta l'impostazione del gruppo datetime.

```csharp
public class DateTimeGroupItem
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DateTimeGroupItem](datetimegroupitem/)(DateTimeGroupingType, int, int, int, int, int, int) |  |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DateTimeGroupingType](../../aspose.cells/datetimegroupitem/datetimegroupingtype/) { get; set; } | Ottiene e imposta il tipo di gruppo. |
| [Day](../../aspose.cells/datetimegroupitem/day/) { get; set; } | Ottiene e imposta il giorno della data/ora raggruppata. |
| [Hour](../../aspose.cells/datetimegroupitem/hour/) { get; set; } | Ottiene e imposta l'ora della data/ora raggruppata. |
| [Minute](../../aspose.cells/datetimegroupitem/minute/) { get; set; } | Ottiene e imposta il minuto della data/ora raggruppata. |
| [MinValue](../../aspose.cells/datetimegroupitem/minvalue/) { get; } | Ottiene il valore minimo. |
| [Month](../../aspose.cells/datetimegroupitem/month/) { get; set; } | Ottiene e imposta il mese della data/ora raggruppata. |
| [Second](../../aspose.cells/datetimegroupitem/second/) { get; set; } | Ottiene e imposta il secondo della data/ora raggruppata. |
| [Year](../../aspose.cells/datetimegroupitem/year/) { get; set; } | Ottiene e imposta l'anno della data/ora raggruppata. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemDemo
    {
        public static void DateTimeGroupItemExample()
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

            // Accesso alle proprietà
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);
            Console.WriteLine("DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Second: " + dateTimeGroupItem.Second);

            // Modifica delle proprietà
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;
            dateTimeGroupItem.Day = 25;
            dateTimeGroupItem.Hour = 10;
            dateTimeGroupItem.Minute = 15;
            dateTimeGroupItem.Second = 30;

            // Accesso alle proprietà modificate
            Console.WriteLine("Modified DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Modified Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


