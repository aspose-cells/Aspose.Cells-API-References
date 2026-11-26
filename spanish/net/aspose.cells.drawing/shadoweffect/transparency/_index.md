---
title: "ShadowEffect.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShadowEffect. Obtiene y establece el grado de transparencia de la sombra. Rango de 0.0 opaco a 1.0 claro"
type: docs
url: /es/net/aspose.cells.drawing/shadoweffect/transparency/
---
## ShadowEffect.Transparency property

Obtiene y establece el grado de transparencia de la sombra. Rango de 0.0 (opaco) a 1.0 (claro).

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
    public class ShadowEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma para demostrar el efecto de sombra
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Obtener el efecto de sombra y establecer propiedades, incluida la Transparencia
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4; // Setting transparency to 40%
            shadow.Distance = 80;
            
            // Guarda el libro de trabajo
            workbook.Save("ShadowEffectDemo.xlsx");
            
            Console.WriteLine("Workbook saved with shadow effect transparency set to 0.4");
        }
    }
}
```

### Ver también

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


