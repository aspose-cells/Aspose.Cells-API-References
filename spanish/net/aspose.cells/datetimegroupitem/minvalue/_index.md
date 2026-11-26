---
title: "DateTimeGroupItem.MinValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DateTimeGroupItem. Obtiene el valor mínimo"
type: docs
url: /es/net/aspose.cells/datetimegroupitem/minvalue/
---
## DateTimeGroupItem.MinValue property

Obtiene el valor mínimo.

```csharp
public DateTime MinValue { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinValueDemo
    {
        public static void Run()
        {
            // Crear una instancia de DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                        // Month
                5,                         // Day
                14,                        // Hour
                30,                        // Minute
                45                         // Second
            );

            // Demostrar la propiedad MinValue
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);

            // Mostrar otras propiedades para contexto
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

### Ver también

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


