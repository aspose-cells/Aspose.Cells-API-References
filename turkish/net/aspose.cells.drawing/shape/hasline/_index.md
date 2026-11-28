---
title: "Shape.HasLine"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin çizgi kenarlığının görünür olup olduğunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/hasline/
---
## Shape.HasLine property

Şeklin çizgi kenarlığının görünür olup olmadığını alır ve ayarlar.

```csharp
public bool HasLine { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHasLineDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir örnek şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // HasLine özelliğini gösterin
            Console.WriteLine("Shape initially has line: " + shape.HasLine);
            
            // Çizgiyi kaldırın
            shape.HasLine = false;
            Console.WriteLine("After setting HasLine to false: " + shape.HasLine);
            
            // Çizgiyi geri ekleyin
            shape.HasLine = true;
            Console.WriteLine("After setting HasLine to true: " + shape.HasLine);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


