---
title: "ReflectionEffect.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReflectionEffect. Obtiene y establece el efecto de reflexión predefinido"
type: docs
url: /es/net/aspose.cells.drawing/reflectioneffect/type/
---
## ReflectionEffect.Type property

Obtiene y establece el efecto de reflexión predefinido.

```csharp
public ReflectionEffectType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Obtén el efecto de reflexión
            ReflectionEffect reflection = shape.Reflection;
            
            // Demuestra la propiedad Type
            Console.WriteLine("Initial reflection type: " + reflection.Type);
            
            // Cambia el tipo de reflexión
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            Console.WriteLine("Updated reflection type: " + reflection.Type);
            
            // Establece otras propiedades de reflexión
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Guarda el libro de trabajo
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Ver también

* enum [ReflectionEffectType](../../reflectioneffecttype/)
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


