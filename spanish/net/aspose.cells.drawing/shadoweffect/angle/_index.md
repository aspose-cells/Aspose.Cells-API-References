---
title: "ShadowEffect.Angle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShadowEffect. Obtiene y establece el ángulo de iluminación. Rango de 0 a 359.9 grados"
type: docs
url: /es/net/aspose.cells.drawing/shadoweffect/angle/
---
## ShadowEffect.Angle property

Obtiene y establece el ángulo de iluminación. Rango de 0 a 359,9 grados.

```csharp
public double Angle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyAngleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma y establecer el ángulo del efecto de sombra
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape.ShadowEffect.Angle = 45;

            // Verificar y mostrar el valor del ángulo
            Console.WriteLine("Shadow Effect Angle: " + shape.ShadowEffect.Angle);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


