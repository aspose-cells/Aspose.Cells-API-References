---
title: "ShapeGuideCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeGuideCollection özelliği. Bir şekil kılavuzunu indeksle alır"
type: docs
url: /tr/net/aspose.cells.drawing/shapeguidecollection/item/
---
## ShapeGuideCollection indexer

İndexe göre bir şekil kılavuzu al.

```csharp
public ShapeGuide this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ayar kılavuzlarını kullanan bir şekil ekle
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

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("ShapeGuideCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeGuide](../../shapeguide/)
* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


