---
title: "ShapePathCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePathCollection özelliği. Bir oluşturma yolunu alır"
type: docs
url: /tr/net/aspose.cells.drawing/shapepathcollection/item/
---
## ShapePathCollection indexer

Bir oluşturma yolunu alır.

```csharp
public ShapePath this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Dönüş Değeri

[`ShapePath`](../../shapepath/) nesnesini döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle özel bir şekil (ilkel olmayan şekil) ekle
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 10, 10, 200, 200, 0, 0);

            // ShapePathCollection'a erişin
            ShapePathCollection shapePaths = customShape.Paths;

            // Yeni bir yol ekle
            int pathIndex = shapePaths.Add();

            // Item özelliğini kullanarak yola eriş
            ShapePath newPath = shapePaths[pathIndex];

            // Çıktı bilgisi
            Console.WriteLine("Path count: " + shapePaths.Count);
            Console.WriteLine("Path segment count: " + newPath.PathSegementList.Count);

            // Çalışma kitabını kaydedin
            workbook.Save("ShapePathCollectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePath](../../shapepath/)
* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


