---
title: "FillFormat.GradientVariant"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Devuelve la variante de degradado para el relleno especificado. Solo se aplica a Excel 2007"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/gradientvariant/
---
## FillFormat.GradientVariant property

Devuelve la variante de degradado para el relleno especificado. Solo se aplica a Excel 2007.

```csharp
public int GradientVariant { get; }
```

### Observaciones

Solo puede ser un valor del 1 al 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 150);
            FillFormat fillFormat = rectangle.Fill;
            
            fillFormat.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 2);
            Console.WriteLine("GradientVariant after SetTwoColorGradient: " + fillFormat.GradientVariant);
            
            fillFormat.SetPresetColorGradient(GradientPresetType.Gold, GradientStyleType.FromCorner, 4);
            Console.WriteLine("GradientVariant after SetPresetColorGradient: " + fillFormat.GradientVariant);
        }
    }
}
```

### Ver también

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


