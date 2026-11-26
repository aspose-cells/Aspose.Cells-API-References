---
title: "ReflectionEffect.RotWithShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReflectionEffect. Obtiene y establece si la reflexión debe rotar con la forma"
type: docs
url: /es/net/aspose.cells.drawing/reflectioneffect/rotwithshape/
---
## ReflectionEffect.RotWithShape property

Obtiene y establece si la reflexión debe rotar con la forma.

```csharp
public bool RotWithShape { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyRotWithShapeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Crea y aplica el efecto de reflexión
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.FullReflection4PtOffset;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Transparency = 0.3;

            // Muestra el valor actual de RotWithShape
            Console.WriteLine("Current RotWithShape value: " + reflection.RotWithShape);

            // Establece RotWithShape a true
            reflection.RotWithShape = true;
            Console.WriteLine("RotWithShape set to: " + reflection.RotWithShape);

            // Rota la forma para demostrar el efecto
            shape.RotationAngle = 45;

            // Guarda el libro de trabajo
            workbook.Save("ReflectionEffectRotWithShapeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


