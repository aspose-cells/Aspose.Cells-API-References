---
title: "DateTimeGroupItem.Year"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DateTimeGroupItem. Obtient et définit l'année de la date et heure groupées"
type: docs
url: /fr/net/aspose.cells/datetimegroupitem/year/
---
## DateTimeGroupItem.Year property

Obtient et définit l'année de la date/heure groupée.

```csharp
public int Year { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyYearDemo
    {
        public static void Run()
        {
            // Créer un DateTimeGroupItem groupé par Année
            DateTimeGroupItem dateTimeGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                1,     // Month (ignored when grouping by Year)
                1,     // Day (ignored)
                0,     // Hour (ignored)
                0,     // Minute (ignored)
                0      // Second (ignored)
            );

            // Afficher la valeur initiale de l'Année
            Console.WriteLine("Initial Year: " + dateTimeGroup.Year);

            // Modifier la propriété Année
            dateTimeGroup.Year = 2024;

            // Afficher la valeur Année modifiée
            Console.WriteLine("Modified Year: " + dateTimeGroup.Year);

            // Démontrer que les autres propriétés sont ignorées lors du groupement par Année
            dateTimeGroup.Month = 12;
            Console.WriteLine("Month value is ignored when grouping by Year: " + dateTimeGroup.Month);
        }
    }
}
```

### Voir aussi

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


