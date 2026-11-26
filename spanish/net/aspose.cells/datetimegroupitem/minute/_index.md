---
title: "DateTimeGroupItem.Minute"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DateTimeGroupItem. Obtiene y establece el minuto del tiempo de fecha agrupado"
type: docs
url: /es/net/aspose.cells/datetimegroupitem/minute/
---
## DateTimeGroupItem.Minute property

Obtiene y establece el minuto del fecha y hora agrupados.

```csharp
public int Minute { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinuteDemo
    {
        public static void Run()
        {
            // Crear un DateTimeGroupItem con valores iniciales
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                10,
                5,
                14,
                30,
                45
            );

            // Mostrar valor inicial del minuto
            Console.WriteLine("Initial Minute: " + dateTimeGroupItem.Minute);

            // Cambiar el valor del minuto
            dateTimeGroupItem.Minute = 15;

            // Mostrar valor del minuto modificado
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);

            // Crear un nuevo DateTimeGroupItem con solo agrupación por minuto
            DateTimeGroupItem minuteGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Minute,
                0, 0, 0, 0, 45, 0
            );

            // Mostrar minuto de la agrupación por minuto
            Console.WriteLine("Minute from Minute Grouping: " + minuteGroup.Minute);
        }
    }
}
```

### Ver también

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


