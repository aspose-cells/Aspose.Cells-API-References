---
title: "ShapeSegmentPathCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeSegmentPathCollection yöntemi. Oluşturma yolunda bir segment yolu ekleyin"
type: docs
url: /tr/net/aspose.cells.drawing/shapesegmentpathcollection/add/
---
## ShapeSegmentPathCollection.Add method

Oluşturma yoluna bir segment yolu ekle.

```csharp
public int Add(ShapePathType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ShapePathType | Yol türü. |

### Dönüş Değeri

Listedeki [`ShapeSegmentPath`](../../shapesegmentpath/) nesnesinin konumunu döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionMethodAddWithShapePathTypeDemo
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
            ShapeSegmentPathCollection segmentList = path.PathSegementList;

            segmentList.Add(ShapePathType.Close);

            // Yol segmentlerinin sayısını göster
            Console.WriteLine("Number of path segments: " + segmentList.Count);

            // Her segmenti yinele ve tipini göster
            foreach (ShapeSegmentPath segment in segmentList)
            {
                Console.WriteLine("Segment type: " + segment.Type);
            }

           
            //serbest form ekle
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Şekil değişikliklerini gözlemlemek için çalışma kitabını kaydedin
            workbook.Save("ShapeSegmentPathCollectionAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


