---
title: "Shape.SetLockedProperty"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Establece la propiedad bloqueada"
type: docs
url: /es/net/aspose.cells.drawing/shape/setlockedproperty/
---
## Shape.SetLockedProperty method

Establece la propiedad locked.

```csharp
public void SetLockedProperty(ShapeLockType type, bool value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ShapeLockType | El tipo bloqueado. |
| valor | Booleano | El valor de la propiedad. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLockedPropertyWithShapeLockTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Demuestre el uso de SetLockedProperty
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);
            shape.SetLockedProperty(ShapeLockType.Selection, false);

            Console.WriteLine("Shape locked properties set successfully.");
        }
    }
}
```

### Ver también

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


