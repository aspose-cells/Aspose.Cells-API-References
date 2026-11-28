---
title: "ShapePath.PathSegementList"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePath özelliği. ShapeSegmentPathCollection listesini alır"
type: docs
url: /tr/net/aspose.cells.drawing/shapepath/pathsegementlist/
---
## ShapePath.PathSegementList property

[`ShapeSegmentPathCollection`](../../shapesegmentpathcollection/) listesini alır

```csharp
[Obsolete("Use ShapePath.PathSegments property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ShapeSegmentPathCollection PathSegementList { get; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ShapePath.PathSegments özelliğini kullanın. Bu özellik Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyPathSegementListDemo
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

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ShapePathPropertyPathSegementListDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeSegmentPathCollection](../../shapesegmentpathcollection/)
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


