---
title: "ShapeSegmentPathCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeSegmentPathCollection özelliği. ShapeSegmentPath nesnesini alır"
type: docs
url: /tr/net/aspose.cells.drawing/shapesegmentpathcollection/item/
---
## ShapeSegmentPathCollection indexer

[`ShapeSegmentPath`](../../shapesegmentpath/) nesnesini alır.

```csharp
public ShapeSegmentPath this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Dönüş Değeri

Bir [`ShapeSegmentPath`](../../shapesegmentpath/) nesnesi döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Yeni bir yol başlat
            path.MoveTo(10, 10);

            // Bir çizgi segmenti çiz.
            path.LineTo(100, 100);

            // PathSegementList özelliğine eriş
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;


            segmentPaths.Add(ShapePathType.Close);

            // Yol segmentlerinin sayısını göster
            Console.WriteLine("Number of path segments: " + segmentPaths.Count);
          
            
            // Item özelliğini okuma örneği göster
            for (int i = 0; i < segmentPaths.Count; i++)
            {
                ShapeSegmentPath segment = segmentPaths[i];
                Console.WriteLine($"Segment {i} type: {segment.Type}");
            }

            //serbest form ekle
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });
            // Çalışma kitabını kaydedin
            workbook.Save("ShapeSegmentPathCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeSegmentPath](../../shapesegmentpath/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


