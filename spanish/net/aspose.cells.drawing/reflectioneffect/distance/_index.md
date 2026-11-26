---
title: "ReflectionEffect.Distance"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReflectionEffect. Obtiene y establece la distancia de la sombra en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/reflectioneffect/distance/
---
## ReflectionEffect.Distance property

Obtiene y establece la distancia de la sombra, en unidades de puntos.

```csharp
public double Distance { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade una forma para probar la reflexión - parámetros fijos para coincidir con la firma del método
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Establecer propiedades de reflexión
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4; // Demonstrating Distance property

            // Guardar y recargar para verificar la persistencia
            string outputPath = "ReflectionEffectDemo.xlsx";
            workbook.Save(outputPath);

            // Recargar para verificar
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Original Distance: " + reflection.Distance);
            Console.WriteLine("Loaded Distance: " + loadedReflection.Distance);
        }
    }
}
```

### Ver también

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


