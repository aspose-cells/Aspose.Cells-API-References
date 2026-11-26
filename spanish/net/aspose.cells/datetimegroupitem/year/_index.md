---
title: "DateTimeGroupItem.Year"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DateTimeGroupItem. Obtiene y establece el año del datetime agrupado"
type: docs
url: /es/net/aspose.cells/datetimegroupitem/year/
---
## DateTimeGroupItem.Year property

Obtiene y establece el año del fecha y hora agrupados.

```csharp
public int Year { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyYearDemo
    {
        public static void Run()
        {
            // Crear un DateTimeGroupItem agrupado por Year
            DateTimeGroupItem dateTimeGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                1,     // Month (ignored when grouping by Year)
                1,     // Day (ignored)
                0,     // Hour (ignored)
                0,     // Minute (ignored)
                0      // Second (ignored)
            );

            // Mostrar el valor inicial de Year
            Console.WriteLine("Initial Year: " + dateTimeGroup.Year);

            // Modificar la propiedad Year
            dateTimeGroup.Year = 2024;

            // Mostrar el valor Year modificado
            Console.WriteLine("Modified Year: " + dateTimeGroup.Year);

            // Demostrar que otras propiedades se ignoran al agrupar por Year
            dateTimeGroup.Month = 12;
            Console.WriteLine("Month value is ignored when grouping by Year: " + dateTimeGroup.Month);
        }
    }
}
```

### Ver también

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


