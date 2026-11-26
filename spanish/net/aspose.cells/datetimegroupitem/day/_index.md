---
title: "DateTimeGroupItem.Day"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DateTimeGroupItem. Obtiene y establece el día del tiempo de fecha agrupado"
type: docs
url: /es/net/aspose.cells/datetimegroupitem/day/
---
## DateTimeGroupItem.Day property

Obtiene y establece el día del fecha y hora agrupados.

```csharp
public int Day { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDayDemo
    {
        public static void Run()
        {
            // Crear un DateTimeGroupItem agrupado por Year
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                10,    // Month
                5,     // Day
                14,    // Hour
                30,    // Minute
                45     // Second
            );

            // Mostrar valor inicial del día
            Console.WriteLine("Initial Day: " + dateTimeGroupItem.Day);

            // Cambiar la propiedad del día
            dateTimeGroupItem.Day = 25;
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);

            // Crear otro DateTimeGroupItem agrupado por Day para demostrar la importancia de la propiedad Day
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

### Ver también

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


