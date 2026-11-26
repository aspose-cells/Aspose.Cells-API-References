---
title: "ReflectionEffect.Size"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReflectionEffect. Obtiene y establece la posición final a lo largo de la rampa de degradado alfa del valor alfa final en unidades de porcentaje"
type: docs
url: /es/net/aspose.cells.drawing/reflectioneffect/size/
---
## ReflectionEffect.Size property

Obtiene y establece la posición final (a lo largo de la rampa de degradado alfa) del valor alfa final, en unidades de porcentaje

```csharp
public double Size { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Establece las propiedades de reflexión incluyendo Size
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4;

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            // Verifica las propiedades de reflexión guardadas
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Reflection Size: " + loadedReflection.Size);
        }
    }
}
```

### Ver también

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


