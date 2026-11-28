---
title: "Sınıf CustomGeometry"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.CustomGeometry sınıfı. Özel bir geometrik şekli temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/customgeometry/
---
## CustomGeometry class

Özel bir geometrik şekli temsil eder.

```csharp
public class CustomGeometry : Geometry
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Paths](../../aspose.cells.drawing/customgeometry/paths/) { get; } | Şekil NotPrimitive bir otomatik şekil olduğunda yol koleksiyonu bilgilerini alır |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Şekil ayar değerlerinin bir koleksiyonunu alır ([`Geometry`](../geometry/) sınıfından devralınmıştır). |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassCustomGeometryDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir NotPrimitive otomatik şekil ekle
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 0, 0, 200, 300);

            // Şekilden CustomGeometry örneğini al
            CustomGeometry customGeometry = shape.Geometry as CustomGeometry;

            // Geometri'nin yol koleksiyonunda yeni bir yol oluştur
            int pathIndex = customGeometry.Paths.Add();
            ShapePath path = customGeometry.Paths[pathIndex];

            // Doğrudan yöntem çağrılarıyla yol segmentleri ekle
            path.MoveTo(0, 0);
            path.LineTo(1000, 0);
            path.LineTo(1000, 1000);
            path.LineTo(0, 1000);
            path.Close();

            // Çalışma kitabını kaydedin
            workbook.Save("CustomGeometryDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Geometry](../geometry/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


