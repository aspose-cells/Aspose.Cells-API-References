---
title: "DateTimeGroupItem.Second"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DateTimeGroupItem. Obtient et définit la seconde du date‑time groupé"
type: docs
url: /fr/net/aspose.cells/datetimegroupitem/second/
---
## DateTimeGroupItem.Second property

Obtient et définit la seconde de la date/heure groupée.

```csharp
public int Second { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertySecondDemo
    {
        public static void Run()
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

            // Afficher la valeur initiale de la seconde
            Console.WriteLine("Initial Second: " + dateTimeGroupItem.Second);

            // Modifier la valeur de la seconde
            dateTimeGroupItem.Second = 50;
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);

            // Créer une autre instance avec une valeur de seconde différente
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

### Voir aussi

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


