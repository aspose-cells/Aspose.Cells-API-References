---
title: "Shape.Reflection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa un objeto ReflectionEffect que especifica el efecto de reflexión para el elemento del gráfico o la forma."
type: docs
url: /es/net/aspose.cells.drawing/shape/reflection/
---
## Shape.Reflection property

Representa un objeto [`ReflectionEffect`](../../reflectioneffect/) que especifica el efecto de reflexión para el elemento del gráfico o la forma.

```csharp
public ReflectionEffect Reflection { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyReflectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Establecer propiedades de reflexión
            ReflectionEffect reflection = shape.Reflection;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Direction = 90;
            reflection.FadeDirection = 90;
            reflection.Size = 50;
            reflection.Transparency = 0.5;
            reflection.Type = ReflectionEffectType.None;

            // Guarda el libro de trabajo
            workbook.Save("ShapeReflectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ReflectionEffect](../../reflectioneffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


