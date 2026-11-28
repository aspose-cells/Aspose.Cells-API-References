---
title: "Enum ShapePathType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ShapePathType enum. Yol segmenti tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shapepathtype/
---
## ShapePathType enumeration

Yol segmenti türünü temsil eder.

```csharp
public enum ShapePathType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| LineTo | `1` | Düz çizgi segmenti |
| CubicBezierCurveTo | `3` | Kübik Bezier eğrisi |
| MoveTo | `0` | Yeni bir yol başlat |
| Close | `128` | Başlangıç POINT ve bitiş POINT aynı değilse, yolun başlangıç POINT'i ile bitiş POINT'ini bağlamak için tek bir düz çizgi çizilir. |
| End | `4` | Mevcut yolun sonu |
| Escape | `5` | Kaçış |
| ArcTo | `6` | Bir yay |
| Unknown | `7` | Bilinmeyen |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Yol tiplerini göstermek için bir şekil oluştur
                Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 10, 10, 200, 200);

                // Özel bir geometri yolu oluştur
                Geometry geometry = shape.Geometry;
                ShapePath path = new ShapePath();

                // Farklı ShapePathType değerlerini göster
                Console.WriteLine("Available ShapePathType values:");
                Console.WriteLine($"LineTo: {ShapePathType.LineTo}");
                Console.WriteLine($"CubicBezierCurveTo: {ShapePathType.CubicBezierCurveTo}");
                Console.WriteLine($"MoveTo: {ShapePathType.MoveTo}");
                Console.WriteLine($"Close: {ShapePathType.Close}");
                Console.WriteLine($"End: {ShapePathType.End}");

                // Bazı yol işlemlerini uygula
                path.MoveTo(10, 10);
                path.LineTo(100, 100);
                path.Close();

                // Çalışma kitabını kaydedin
                workbook.Save("ShapePathTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathType: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


