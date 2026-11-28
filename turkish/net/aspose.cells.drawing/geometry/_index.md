---
title: "Sınıf Geometry"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Geometry sınıfı. Geometrik bir şekli temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/geometry/
---
## Geometry class

Geometrik bir şekli temsil eder.

```csharp
public abstract class Geometry
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Şekil ayar değeri koleksiyonunu alır |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    
    public class DrawingClassGeometryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir dikdörtgen şekli ekle
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Şeklin geometrisine eriş
            Geometry geometry = rectangle.Geometry;

            // Şekil ayar kılavuzlarını doğrudan koleksiyona ekle
            geometry.ShapeAdjustValues.Add("Roundness", 0.3);
            geometry.ShapeAdjustValues.Add("Angle", 45.0);

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("GeometryDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


