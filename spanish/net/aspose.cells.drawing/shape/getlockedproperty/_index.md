---
title: "Shape.GetLockedProperty"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Obtiene el valor de la propiedad bloqueada"
type: docs
url: /es/net/aspose.cells.drawing/shape/getlockedproperty/
---
## Shape.GetLockedProperty method

Obtiene el valor de la propiedad locked.

```csharp
public bool GetLockedProperty(ShapeLockType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ShapeLockType | El tipo de la propiedad bloqueada de la forma. |

### Valor de retorno

Devuelve el valor de la propiedad bloqueada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLockedPropertyWithShapeLockTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Establecer la propiedad bloqueada para AdjustHandles
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);

            // Comprobar si AdjustHandles está bloqueado
            int noAdjustHandles = 0;
            if (shape.GetLockedProperty(ShapeLockType.AdjustHandles))
                noAdjustHandles = 1;

            Console.WriteLine("AdjustHandles locked status: " + (noAdjustHandles == 1));
        }
    }
}
```

### Ver también

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


