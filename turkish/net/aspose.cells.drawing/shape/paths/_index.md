---
title: "Shape.Paths"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Şekil özelliği. Özel bir geometrik şeklin yollarını alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/paths/
---
## Shape.Paths property

Özel bir geometrik şeklin yollarını alır.

```csharp
public ShapePathCollection Paths { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPathsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir özel şekil (dikdörtgen) ekle
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 1, 1, 100, 150);

            // Şeklin özel geometri yolları olup olmadığını kontrol et
            if (shape.Paths != null)
            {
                Console.WriteLine("Shape has custom geometry paths:");
                Console.WriteLine($"Number of paths: {shape.Paths.Count}");
                
                // Şeklin geometrisine yeni bir yol ekle
                int newPathIndex = shape.Paths.Add();
                Console.WriteLine($"Added new path at index: {newPathIndex}");
            }
            else
            {
                Console.WriteLine("No custom geometry path.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePathCollection](../../shapepathcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


