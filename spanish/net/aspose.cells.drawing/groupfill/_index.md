---
title: "Clase GroupFill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.GroupFill class. Representa que este formato de relleno debe heredar las propiedades de relleno del grupo"
type: docs
url: /es/net/aspose.cells.drawing/groupfill/
---
## GroupFill class

Representa que este formato de relleno debe heredar las propiedades de relleno del grupo.

```csharp
public class GroupFill : Fill
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Hereda de [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Obtiene el código hash.(Hereda de [`Fill`](../fill/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGroupFillDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // GroupFill no expone un constructor público sin parámetros.
                // Para propósitos de demostración obtenemos una referencia (null) del tipo.
                GroupFill groupFill = null;

                // Muestre que la variable de tipo GroupFill existe.
                Console.WriteLine($"GroupFill variable declared. Type: {typeof(GroupFill).FullName}");

                // Guarde el libro de trabajo (aunque no lo modificamos, esto demuestra un flujo de trabajo completo)
                workbook.Save("GroupFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GroupFill: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


