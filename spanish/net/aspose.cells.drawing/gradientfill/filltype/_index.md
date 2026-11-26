---
title: "GradientFill.FillType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GradientFill. Obtiene el tipo de relleno del degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientfill/filltype/
---
## GradientFill.FillType property

Obtiene el tipo de relleno degradado.

```csharp
public GradientFillType FillType { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma con relleno degradado
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            FillFormat fillFormat = shape.Fill;
            fillFormat.FillType = FillType.Gradient;
            
            // Establecer propiedades del degradado
            GradientFill gradientFill = fillFormat.GradientFill;
            gradientFill.SetTwoColorGradient(System.Drawing.Color.Red, System.Drawing.Color.Blue, GradientStyleType.Horizontal, 1);
            
            // Mostrar el tipo de relleno del degradado
            Console.WriteLine("Gradient Fill Type: " + gradientFill.FillType);
            
            // Cambiar a degradado radial
            gradientFill.SetGradient(GradientFillType.Radial, 45, GradientDirectionType.FromCenter);
            Console.WriteLine("Updated Gradient Fill Type: " + gradientFill.FillType);
            
            // Guarda el libro de trabajo
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientFillType](../../gradientfilltype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


