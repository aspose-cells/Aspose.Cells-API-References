---
title: "Enumeración LightRigDirectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.LightRigDirectionType enum. Representa el tipo de dirección del rig de luz"
type: docs
url: /es/net/aspose.cells.drawing/lightrigdirectiontype/
---
## LightRigDirectionType enumeration

Representa el tipo de dirección del rig de luz.

```csharp
public enum LightRigDirectionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Bottom | `0` | Inferior |
| BottomLeft | `1` | Inferior izquierda. |
| BottomRight | `2` | Inferior derecha. |
| Left | `3` | Izquierda. |
| Right | `4` | Derecha. |
| Top | `5` | Arriba. |
| TopLeft | `6` | Superior izquierda. |
| TopRight | `7` | Arriba a la derecha. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassLightRigDirectionTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar la dirección del rig de luz
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 200, 0, 0);

            // Establecer la dirección del rig de luz para el formato 3D de la forma
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.TopRight;

            // Demostrar diferentes direcciones del rig de luz
            Console.WriteLine("Current Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Cambiar la dirección del rig de luz
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.BottomLeft;
            Console.WriteLine("Changed Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Iterar a través de todas las direcciones posibles del rig de luz
            Console.WriteLine("\nAll Light Rig Direction Types:");
            foreach (LightRigDirectionType direction in Enum.GetValues(typeof(LightRigDirectionType)))
            {
                Console.WriteLine(direction.ToString());
            }

            // Guarda el libro de trabajo
            workbook.Save("LightRigDirectionTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


