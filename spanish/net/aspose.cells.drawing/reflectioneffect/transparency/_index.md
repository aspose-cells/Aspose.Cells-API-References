---
title: "ReflectionEffect.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ReflectionEffect. Obtiene y establece el grado de transparencia inicial de la reflexión como un valor de 0.0 opaco a 1.0 claro"
type: docs
url: /es/net/aspose.cells.drawing/reflectioneffect/transparency/
---
## ReflectionEffect.Transparency property

Obtiene y establece el grado de transparencia inicial de la reflexión como un valor de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Añade una forma rectangular a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 150);
            
            // Obtén el efecto de reflexión y establece sus propiedades
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5; // Demonstrate transparency property
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Guarda el libro de trabajo
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Verificar las propiedades guardadas
            Workbook loadedWorkbook = new Workbook("ReflectionEffectDemo.xlsx");
            Aspose.Cells.Drawing.ReflectionEffect loadedReflection = loadedWorkbook.Worksheets[0].Shapes[0].Reflection;
            
            Console.WriteLine("Reflection Type: " + loadedReflection.Type);
            Console.WriteLine("Transparency: " + loadedReflection.Transparency);
            Console.WriteLine("Size: " + loadedReflection.Size);
            Console.WriteLine("Blur: " + loadedReflection.Blur);
            Console.WriteLine("Distance: " + loadedReflection.Distance);
        }
    }
}
```

### Ver también

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


