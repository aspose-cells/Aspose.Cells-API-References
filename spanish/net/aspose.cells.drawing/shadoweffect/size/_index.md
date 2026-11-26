---
title: "ShadowEffect.Size"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShadowEffect. Obtiene y establece el tamaño de la sombra. Rango de 0 a 2.0. Sin sentido en sombra interna"
type: docs
url: /es/net/aspose.cells.drawing/shadoweffect/size/
---
## ShadowEffect.Size property

Obtiene y establece el tamaño de la sombra. Rango de 0 a 2.0. No tiene sentido en sombra interna.

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
    public class ShadowEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook book = new Workbook();
            
            // Acceder a la primera hoja de cálculo y agregar una forma
            Worksheet sheet = book.Worksheets[0];
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Obtener el efecto de sombra y establecer propiedades, incluido el Tamaño
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3; // Demonstrating Size property usage
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Guarda el libro de trabajo
            book.Save("ShadowEffectExample.xlsx");
            
            Console.WriteLine("Shadow effect with Size property set to 1.3 has been applied.");
        }
    }
}
```

### Ver también

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


