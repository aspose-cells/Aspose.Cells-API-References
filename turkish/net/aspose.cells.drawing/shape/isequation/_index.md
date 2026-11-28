---
title: "Shape.IsEquation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin yalnızca bir denklem içerip içermediğini gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/isequation/
---
## Shape.IsEquation property

Şeklin yalnızca bir denklem içerip içermediğini gösterir.

```csharp
public bool IsEquation { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsEquationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir denklem şekli ekle
            Shape equationShape = worksheet.Shapes.AddEquation(0, 0, 0, 0, 100, 100);
            equationShape.AlternativeText = "x^2 + y^2 = r^2";
            
            // Doğru parametrelerle normal bir dikdörtgen şekli ekle
            Shape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 0, 0, 100, 100);

            foreach (Shape shape in worksheet.Shapes)
            {
                if (shape.IsEquation)
                {
                    Console.WriteLine("Shape is an equation: " + shape.AlternativeText);
                }
                else
                {
                    Console.WriteLine("Shape is not an equation");
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


