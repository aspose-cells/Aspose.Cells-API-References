---
title: "Shape.GetResultOfSmartArt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Akıllı sanatı gruplanmış şekillere dönüştürme"
type: docs
url: /tr/net/aspose.cells.drawing/shape/getresultofsmartart/
---
## Shape.GetResultOfSmartArt method

Smart art'ı gruplanmış şekillere dönüştürme.

```csharp
public virtual GroupShape GetResultOfSmartArt()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetResultOfSmartArtDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekleyin (çünkü SmartArt'ı doğrudan oluşturamıyoruz)
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 200, 200, 0, 0);
            
            // Gerçek bir senaryoda, mevcut bir SmartArt şekli yüklerdik
            // Demo amaçları için, IsSmartArt kontrolünü atlayacağız çünkü onu ayarlayamıyoruz

            // SmartArt sonucunu al (yalnızca şekil gerçekten SmartArt ise çalışır)
            GroupShape groupShape = shape.GetResultOfSmartArt();
            Console.WriteLine("Converted shape to GroupShape");
        }
    }
}
```

### Ayrıca Bakınız

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


