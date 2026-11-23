---
title: "DateTimeGroupItem.MinValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DateTimeGroupItem. Obtient la valeur minimale"
type: docs
url: /fr/net/aspose.cells/datetimegroupitem/minvalue/
---
## DateTimeGroupItem.MinValue property

Obtient la valeur minimale.

```csharp
public DateTime MinValue { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinValueDemo
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

            // Démontrer la propriété MinValue
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);

            // Afficher d'autres propriétés pour le contexte
            Console.WriteLine("Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Date Components: {0}-{1}-{2} {3}:{4}:{5}",
                dateTimeGroupItem.Year,
                dateTimeGroupItem.Month,
                dateTimeGroupItem.Day,
                dateTimeGroupItem.Hour,
                dateTimeGroupItem.Minute,
                dateTimeGroupItem.Second);
        }
    }
}
```

### Voir aussi

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


