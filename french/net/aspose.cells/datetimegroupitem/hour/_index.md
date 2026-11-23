---
title: "DateTimeGroupItem.Hour"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DateTimeGroupItem. Obtient et définit l'heure du date-time groupé"
type: docs
url: /fr/net/aspose.cells/datetimegroupitem/hour/
---
## DateTimeGroupItem.Hour property

Obtient et définit l'heure de la date/heure groupée.

```csharp
public int Hour { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyHourDemo
    {
        public static void Run()
        {
            // Créer un DateTimeGroupItem avec regroupement par heure
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Hour,
                2023,  // Year
                10,     // Month
                5,      // Day
                14,     // Hour
                0,      // Minute
                0      // Second
            );

            // Afficher la valeur d'heure initiale
            Console.WriteLine("Initial Hour: " + dateTimeGroupItem.Hour);

            // Modifier la propriété hour
            dateTimeGroupItem.Hour = 18;

            // Afficher la valeur hour modifiée
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
        }
    }
}
```

### Voir aussi

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


