---
title: "ShapeGuide.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeGuide özelliği. Bu kılavuzun değerini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shapeguide/value/
---
## ShapeGuide.Value property

Bu kılavuzun değerini alır veya ayarlar

```csharp
public double Value { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuidePropertyValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ayar kılavuzlarını kullanan bir şekil oluştur
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            
            // Geometri aracılığıyla şeklin ayar kılavuzları koleksiyonuna eriş
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

            // Koleksiyona yeni kılavuzlar ekle
            shapeGuides.Add("adj1", 25.5);
            shapeGuides.Add("adj2", 30);
            shapeGuides.Add("adj3", 25.5);
            shapeGuides.Add("adj4", 35);

            // Kılavuz değerlerini okuma gösterimi (Name özelliği sağlanan tanımda mevcut değil)
            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);


            Console.WriteLine("Updated adjustment values");

            shapeGuides[0].Value = 25.5;
            shapeGuides[1].Value = 25.5;
            shapeGuides[2].Value = 25.5;
            shapeGuides[3].Value = 25.5;            

            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);
            
            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("ShapeGuideValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeGuide](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


