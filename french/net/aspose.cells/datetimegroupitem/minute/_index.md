---
title: "DateTimeGroupItem.Minute"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DateTimeGroupItem. Obtient et définit la minute de la date et heure groupées"
type: docs
url: /fr/net/aspose.cells/datetimegroupitem/minute/
---
## DateTimeGroupItem.Minute property

Obtient et définit la minute de la date/heure groupée.

```csharp
public int Minute { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinuteDemo
    {
        public static void Run()
        {
            // Créer un DateTimeGroupItem avec des valeurs initiales
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                10,
                5,
                14,
                30,
                45
            );

            // Afficher la valeur initiale de la minute
            Console.WriteLine("Initial Minute: " + dateTimeGroupItem.Minute);

            // Modifier la valeur de la minute
            dateTimeGroupItem.Minute = 15;

            // Afficher la valeur de la minute modifiée
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);

            // Créer un nouveau DateTimeGroupItem avec uniquement le regroupement par minute
            DateTimeGroupItem minuteGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Minute,
                0, 0, 0, 0, 45, 0
            );

            // Afficher la minute du regroupement par minute
            Console.WriteLine("Minute from Minute Grouping: " + minuteGroup.Minute);
        }
    }
}
```

### Voir aussi

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


