---
title: "Classe DateTimeGroupItem"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.DateTimeGroupItem. Représente le paramètre de groupe de date/heure"
type: docs
url: /fr/net/aspose.cells/datetimegroupitem/
---
## DateTimeGroupItem class

Représente le paramètre de groupe de date et heure.

```csharp
public class DateTimeGroupItem
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DateTimeGroupItem](datetimegroupitem/)(DateTimeGroupingType, int, int, int, int, int, int) |  |

## Propriétés

| Nom | Description |
| --- | --- |
| [DateTimeGroupingType](../../aspose.cells/datetimegroupitem/datetimegroupingtype/) { get; set; } | Obtient et définit le type de groupe. |
| [Day](../../aspose.cells/datetimegroupitem/day/) { get; set; } | Obtient et définit le jour de la date/heure groupée. |
| [Hour](../../aspose.cells/datetimegroupitem/hour/) { get; set; } | Obtient et définit l'heure de la date/heure groupée. |
| [Minute](../../aspose.cells/datetimegroupitem/minute/) { get; set; } | Obtient et définit la minute de la date/heure groupée. |
| [MinValue](../../aspose.cells/datetimegroupitem/minvalue/) { get; } | Obtient la valeur minimale. |
| [Month](../../aspose.cells/datetimegroupitem/month/) { get; set; } | Obtient et définit le mois de la date/heure groupée. |
| [Second](../../aspose.cells/datetimegroupitem/second/) { get; set; } | Obtient et définit la seconde de la date/heure groupée. |
| [Year](../../aspose.cells/datetimegroupitem/year/) { get; set; } | Obtient et définit l'année de la date/heure groupée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemDemo
    {
        public static void DateTimeGroupItemExample()
        {
            // Créez une instance de DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                        // Month
                5,                         // Day
                14,                        // Hour
                30,                        // Minute
                45                         // Second
            );

            // Accès aux propriétés
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);
            Console.WriteLine("DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Second: " + dateTimeGroupItem.Second);

            // Modification des propriétés
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;
            dateTimeGroupItem.Day = 25;
            dateTimeGroupItem.Hour = 10;
            dateTimeGroupItem.Minute = 15;
            dateTimeGroupItem.Second = 30;

            // Accès aux propriétés modifiées
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

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


