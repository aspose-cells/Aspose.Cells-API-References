---
title: "ShapeSegmentPath.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeSegmentPath özelliği. Yol segmentinin tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing/shapesegmentpath/type/
---
## ShapeSegmentPath.Type property

Yol segment tipi alır

```csharp
public ShapePathType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Yeni bir şekil yolu oluştur
                ShapePath shapePath = new ShapePath();

                // Başlangıç noktasına git
                shapePath.MoveTo(10, 10);

                // (Single, Single) parametreleriyle LineTo yöntemini çağır
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                // PathSegementList özelliğine eriş
                ShapeSegmentPathCollection segmentList = shapePath.PathSegementList;

                // Yol segmentlerinin sayısını göster
                Console.WriteLine("Number of path segments: " + segmentList.Count);

                // Her segmenti yinele ve tipini göster
                foreach (ShapeSegmentPath segment in segmentList)
                {
                    Console.WriteLine("Segment type: " + segment.Type);
                }

                //serbest form ekle
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }


            // Çalışma kitabını kaydedin
            workbook.Save("ShapeSegmentPathTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


