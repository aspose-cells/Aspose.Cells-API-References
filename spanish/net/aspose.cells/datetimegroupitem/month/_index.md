---
title: "DateTimeGroupItem.Month"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DateTimeGroupItem. Obtiene y establece el mes del tiempo de fecha agrupado"
type: docs
url: /es/net/aspose.cells/datetimegroupitem/month/
---
## DateTimeGroupItem.Month property

Obtiene y establece el mes del fecha y hora agrupados.

```csharp
public int Month { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMonthDemo
    {
        public static void Run()
        {
            // Crear un DateTimeGroupItem agrupado por Month
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Month,
                2023,
                10,
                1,
                0,
                0,
                0
            );

            // Mostrar valor inicial del mes
            Console.WriteLine("Initial Month: " + dateTimeGroupItem.Month);

            // Cambiar el valor del mes
            dateTimeGroupItem.Month = 12;
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);

            // Crear otro DateTimeGroupItem con una agrupación diferente
            DateTimeGroupItem yearlyItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                1,
                1,
                0,
                0,
                0
            );

            // Mostrar que la propiedad Month sigue siendo accesible incluso cuando está agrupada por Year
            Console.WriteLine("Yearly Grouping - Month: " + yearlyItem.Month);
        }
    }
}
```

### Ver también

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


