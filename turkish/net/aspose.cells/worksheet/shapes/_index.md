---
title: "Worksheet.Shapes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bu çalışma sayfasındaki tüm çizim şekillerini döndürür"
type: docs
url: /tr/net/aspose.cells/worksheet/shapes/
---
## Worksheet.Shapes property

Bu çalışma sayfasındaki tüm çizim şekillerini döndürür.

```csharp
public ShapeCollection Shapes { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShapesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bazı şekiller ekleyin
            sheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            sheet.Shapes.AddLine(2, 0, 100, 100, 100, 1);
            
            // Şekil özelliklerini değiştirin
            for (int i = 0; i < sheet.Shapes.Count; i++)
            {
                Aspose.Cells.Drawing.Shape shape = sheet.Shapes[i];
                Console.WriteLine($"Shape {i}: Type={shape.Type}, Name={shape.Name}");
                
                // İlk şeklin özelliklerini güncelleyin
                if (i == 0)
                {
                    shape.Name = "MyRectangle";
                    shape.FillFormat.ForeColor = System.Drawing.Color.Red;
                }
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ShapesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


