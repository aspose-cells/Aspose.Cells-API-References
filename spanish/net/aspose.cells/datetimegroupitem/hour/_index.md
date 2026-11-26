---
title: "DateTimeGroupItem.Hour"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DateTimeGroupItem. Obtiene y establece la hora del datetime agrupado"
type: docs
url: /es/net/aspose.cells/datetimegroupitem/hour/
---
## DateTimeGroupItem.Hour property

Obtiene y establece la hora del fecha y hora agrupados.

```csharp
public int Hour { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyHourDemo
    {
        public static void Run()
        {
            // Crear un DateTimeGroupItem con agrupación por hora
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Hour,
                2023,  // Year
                10,     // Month
                5,      // Day
                14,     // Hour
                0,      // Minute
                0      // Second
            );

            // Mostrar valor de hora inicial
            Console.WriteLine("Initial Hour: " + dateTimeGroupItem.Hour);

            // Modificar la propiedad hour
            dateTimeGroupItem.Hour = 18;

            // Mostrar el valor hour modificado
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
        }
    }
}
```

### Ver también

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


