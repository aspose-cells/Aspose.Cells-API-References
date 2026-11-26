---
title: "ReflectionEffect.Blur"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReflectionEffect. Obtiene y establece el radio de desenfoque en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/reflectioneffect/blur/
---
## ReflectionEffect.Blur property

Obtiene y establece el radio de desenfoque, en unidades de puntos.

```csharp
public double Blur { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma rectangular
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Accede al efecto de reflexión
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            
            // Establece el tipo y las propiedades de reflexión
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Blur = 0.5; // Demonstrate Blur property
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Distance = 0;
            
            // Guarda el libro de trabajo
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Muestra el valor de desenfoque
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
        }
    }
}
```

### Ver también

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


