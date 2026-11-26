---
title: "DateTimeGroupItem.DateTimeGroupingType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DateTimeGroupItem. Obtiene y establece el tipo de grupo"
type: docs
url: /es/net/aspose.cells/datetimegroupitem/datetimegroupingtype/
---
## DateTimeGroupItem.DateTimeGroupingType property

Obtiene y establece el tipo de grupo.

```csharp
public DateTimeGroupingType DateTimeGroupingType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDateTimeGroupingTypeDemo
    {
        public static void Run()
        {
            // Crear una instancia de DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                       // Month
                5,                         // Day
                14,                       // Hour
                30,                       // Minute
                45                        // Second
            );

            // Mostrar propiedades iniciales
            Console.WriteLine("Initial Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine($"Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}-{dateTimeGroupItem.Day}");

            // Cambiar el tipo de agrupación y los componentes de fecha
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;

            // Mostrar propiedades modificadas
            Console.WriteLine("Modified Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine($"Modified Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}");
        }
    }
}
```

### Ver también

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


