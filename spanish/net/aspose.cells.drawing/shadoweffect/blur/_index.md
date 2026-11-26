---
title: "ShadowEffect.Blur"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShadowEffect. Obtiene y establece el desenfoque de la sombra. Rango de 0 a 100 puntos"
type: docs
url: /es/net/aspose.cells.drawing/shadoweffect/blur/
---
## ShadowEffect.Blur property

Obtiene y establece el desenfoque de la sombra. Rango de 0 a 100 puntos.

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
    public class ShadowEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma de ejemplo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Obtener efecto de sombra
            ShadowEffect shadow = shape.ShadowEffect;
            
            // Establecer propiedades de sombra, incluido el Desenfoque
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Shadow effect with blur applied successfully.");
        }
    }
}
```

### Ver también

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


