---
title: "DateTimeGroupItem.Month"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DateTimeGroupItem. Obtient et définit le mois de la date et heure groupées"
type: docs
url: /fr/net/aspose.cells/datetimegroupitem/month/
---
## DateTimeGroupItem.Month property

Obtient et définit le mois de la date/heure groupée.

```csharp
public int Month { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMonthDemo
    {
        public static void Run()
        {
            // Créer un DateTimeGroupItem groupé par Month
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Month,
                2023,
                10,
                1,
                0,
                0,
                0
            );

            // Afficher la valeur initiale du mois
            Console.WriteLine("Initial Month: " + dateTimeGroupItem.Month);

            // Modifier la valeur du mois
            dateTimeGroupItem.Month = 12;
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);

            // Créer un autre DateTimeGroupItem avec un regroupement différent
            DateTimeGroupItem yearlyItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                1,
                1,
                0,
                0,
                0
            );

            // Montrer que la propriété Month est toujours accessible même lorsqu'elle est groupée par Year
            Console.WriteLine("Yearly Grouping - Month: " + yearlyItem.Month);
        }
    }
}
```

### Voir aussi

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


