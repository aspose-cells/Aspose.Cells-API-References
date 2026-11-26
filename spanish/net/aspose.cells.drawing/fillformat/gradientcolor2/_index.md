---
title: "FillFormat.GradientColor2"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Devuelve el color de degradado 2 para el relleno especificado"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/gradientcolor2/
---
## FillFormat.GradientColor2 property

Devuelve el color de degradado 2 para el relleno especificado.

```csharp
public Color GradientColor2 { get; }
```

### Observaciones

Solo cuando el tipo de color de degradado es GradientColorType.TwoColors, esta propiedad tiene sentido.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientColor2Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear forma rectangular con relleno de degradado de dos colores
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fill = rectangle.Fill;
            
            fill.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 2);

            // Verificar propiedades del color de degradado
            Console.WriteLine("GradientColor2: " + fill.GradientColor2);
        }
    }
}
```

### Ver también

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


