---
title: "Clase DateTimeGroupItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DateTimeGroupItem. Representa la configuración del grupo de fecha y hora"
type: docs
url: /es/net/aspose.cells/datetimegroupitem/
---
## DateTimeGroupItem class

Representa la configuración del grupo de fecha y hora.

```csharp
public class DateTimeGroupItem
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DateTimeGroupItem](datetimegroupitem/)(DateTimeGroupingType, int, int, int, int, int, int) |  |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DateTimeGroupingType](../../aspose.cells/datetimegroupitem/datetimegroupingtype/) { get; set; } | Obtiene y establece el tipo de grupo. |
| [Day](../../aspose.cells/datetimegroupitem/day/) { get; set; } | Obtiene y establece el día del fecha y hora agrupados. |
| [Hour](../../aspose.cells/datetimegroupitem/hour/) { get; set; } | Obtiene y establece la hora del fecha y hora agrupados. |
| [Minute](../../aspose.cells/datetimegroupitem/minute/) { get; set; } | Obtiene y establece el minuto del fecha y hora agrupados. |
| [MinValue](../../aspose.cells/datetimegroupitem/minvalue/) { get; } | Obtiene el valor mínimo. |
| [Month](../../aspose.cells/datetimegroupitem/month/) { get; set; } | Obtiene y establece el mes del fecha y hora agrupados. |
| [Second](../../aspose.cells/datetimegroupitem/second/) { get; set; } | Obtiene y establece el segundo del fecha y hora agrupados. |
| [Year](../../aspose.cells/datetimegroupitem/year/) { get; set; } | Obtiene y establece el año del fecha y hora agrupados. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemDemo
    {
        public static void DateTimeGroupItemExample()
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

            // Accediendo a propiedades
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);
            Console.WriteLine("DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Second: " + dateTimeGroupItem.Second);

            // Modificando propiedades
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;
            dateTimeGroupItem.Day = 25;
            dateTimeGroupItem.Hour = 10;
            dateTimeGroupItem.Minute = 15;
            dateTimeGroupItem.Second = 30;

            // Accediendo a propiedades modificadas
            Console.WriteLine("Modified DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Modified Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


