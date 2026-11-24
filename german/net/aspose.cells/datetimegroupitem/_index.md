---
title: "Klasse DateTimeGroupItem"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DateTimeGroupItem Klasse. Stellt die Datum‑Uhrzeit‑Gruppeneinstellung dar"
type: docs
url: /de/net/aspose.cells/datetimegroupitem/
---
## DateTimeGroupItem class

Stellt die Datumszeit-Gruppeneinstellung dar.

```csharp
public class DateTimeGroupItem
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [DateTimeGroupItem](datetimegroupitem/)(DateTimeGroupingType, int, int, int, int, int, int) |  |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DateTimeGroupingType](../../aspose.cells/datetimegroupitem/datetimegroupingtype/) { get; set; } | Liest und setzt den Gruppentyp. |
| [Day](../../aspose.cells/datetimegroupitem/day/) { get; set; } | Liest und setzt den Tag der gruppierten Datum‑Uhrzeit. |
| [Hour](../../aspose.cells/datetimegroupitem/hour/) { get; set; } | Liest und setzt die Stunde der gruppierten Datum‑Uhrzeit. |
| [Minute](../../aspose.cells/datetimegroupitem/minute/) { get; set; } | Liest und setzt die Minute der gruppierten Datum‑Uhrzeit. |
| [MinValue](../../aspose.cells/datetimegroupitem/minvalue/) { get; } | Liest den Minimalwert. |
| [Month](../../aspose.cells/datetimegroupitem/month/) { get; set; } | Liest und setzt den Monat der gruppierten Datum‑Uhrzeit. |
| [Second](../../aspose.cells/datetimegroupitem/second/) { get; set; } | Liest und setzt die Sekunde der gruppierten Datum‑Uhrzeit. |
| [Year](../../aspose.cells/datetimegroupitem/year/) { get; set; } | Liest und setzt das Jahr der gruppierten Datum‑Uhrzeit. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemDemo
    {
        public static void DateTimeGroupItemExample()
        {
            // Erstelle eine Instanz von DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                        // Month
                5,                         // Day
                14,                        // Hour
                30,                        // Minute
                45                         // Second
            );

            // Zugriff auf Eigenschaften
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);
            Console.WriteLine("DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Second: " + dateTimeGroupItem.Second);

            // Eigenschaften ändern
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;
            dateTimeGroupItem.Day = 25;
            dateTimeGroupItem.Hour = 10;
            dateTimeGroupItem.Minute = 15;
            dateTimeGroupItem.Second = 30;

            // Zugriff auf geänderte Eigenschaften
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

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


