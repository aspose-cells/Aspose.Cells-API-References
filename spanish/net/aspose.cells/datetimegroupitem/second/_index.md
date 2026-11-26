---
title: "DateTimeGroupItem.Second"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DateTimeGroupItem. Obtiene y establece el segundo de la fecha y hora agrupada"
type: docs
url: /es/net/aspose.cells/datetimegroupitem/second/
---
## DateTimeGroupItem.Second property

Obtiene y establece el segundo del fecha y hora agrupados.

```csharp
public int Second { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertySecondDemo
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

            // Mostrar el valor inicial del segundo
            Console.WriteLine("Initial Second: " + dateTimeGroupItem.Second);

            // Modificar el valor del segundo
            dateTimeGroupItem.Second = 50;
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);

            // Crear otra instancia con un valor de segundo diferente
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

### Ver también

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


