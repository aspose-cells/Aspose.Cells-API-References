---
title: "CustomGeometry.Paths"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomGeometry özelliği. Şekil NotPrimitive bir otomatik şekil olduğunda yol koleksiyonu bilgilerini alır"
type: docs
url: /tr/net/aspose.cells.drawing/customgeometry/paths/
---
## CustomGeometry.Paths property

Şekil NotPrimitive bir otomatik şekil olduğunda yol koleksiyonu bilgilerini alır

```csharp
public ShapePathCollection Paths { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CustomGeometryPropertyPathsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sabit parametrelerle, ilkel olmayan geometriye sahip bir özel şekil ekle
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 10, 10, 400, 400);
            
            // Özel geometriye açık dönüşümle erişin
            CustomGeometry geometry = (CustomGeometry)shape.Geometry;
            
            // Yol koleksiyonunu al
            ShapePathCollection paths = geometry.Paths;
            Console.WriteLine($"Initial path count: {paths.Count}");

            // Çizim komutları kullanarak yeni bir şekil yolu oluştur
            paths.Add(); // Creates a new path in the collection
            ShapePath newPath = paths[paths.Count - 1];
            newPath.MoveTo(0, 0);
            newPath.LineTo(10000, 0);
            newPath.LineTo(10000, 10000);
            newPath.LineTo(0, 10000);
            newPath.Close();

            // Yol koleksiyonda oluşturulduğu için açık bir Add gerekmez
            Console.WriteLine($"New path count after modification: {paths.Count}");

            // Kalıcı değişiklikleri göstermek için kaydet
            workbook.Save("CustomGeometryPathsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePathCollection](../../shapepathcollection/)
* class [CustomGeometry](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


