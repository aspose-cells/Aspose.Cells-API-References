---
title: "DateTimeGroupItem.Day"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DateTimeGroupItem. Obtient et définit le jour de la date et heure groupées"
type: docs
url: /fr/net/aspose.cells/datetimegroupitem/day/
---
## DateTimeGroupItem.Day property

Obtient et définit le jour de la date/heure groupée.

```csharp
public int Day { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDayDemo
    {
        public static void Run()
        {
            // Créer un DateTimeGroupItem groupé par Année
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                10,    // Month
                5,     // Day
                14,    // Hour
                30,    // Minute
                45     // Second
            );

            // Afficher la valeur initiale du jour
            Console.WriteLine("Initial Day: " + dateTimeGroupItem.Day);

            // Modifier la propriété du jour
            dateTimeGroupItem.Day = 25;
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);

            // Créer un autre DateTimeGroupItem groupé par Day pour démontrer l'importance de la propriété Day
            DateTimeGroupItem dayGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Day,
                2023,
                10,
                15,  // Initial day
                0,
                0,
                0
            );

            Console.WriteLine("\nDay-grouped item initial Day: " + dayGroupItem.Day);
            dayGroupItem.Day = 20;
            Console.WriteLine("Day-grouped item modified Day: " + dayGroupItem.Day);
        }
    }
}
```

### Voir aussi

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


