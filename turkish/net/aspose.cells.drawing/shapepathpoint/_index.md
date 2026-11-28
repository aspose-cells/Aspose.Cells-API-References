---
title: "Sınıf ShapePathPoint"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ShapePathPoint sınıfı. Konum koordinatlarını veya açı işaretçilerini belirtir. Konum koordinatları, bir yolun koordinat uzayındaki koordinatlarını (ör. X/Y) temsil eder. Açı işaretçileri, bir yol üzerindeki açısal değişimleri (ör. bir yayının başlangıç ve salınım açıları) gösterir."
type: docs
url: /tr/net/aspose.cells.drawing/shapepathpoint/
---
## ShapePathPoint class

Pozisyon koordinatlarını veya açı işaretçilerini belirtin. Pozisyon koordinatları, bir koordinat uzayındaki (ör. X/Y) yolun koordinatlarını temsil eder. Açı işaretçileri, bir yoldaki açısal değişiklikleri gösterir (ör. bir yayının başlangıç ve salınım açıları).

```csharp
public class ShapePathPoint
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Type](../../aspose.cells.drawing/shapepathpoint/type/) { get; } | Geçerli nesnenin değer tipini belirtir. |
| [X](../../aspose.cells.drawing/shapepathpoint/x/) { get; set; } | (**Obsolete.**) Bu konum koordinatı için x koordinatını alır ve ayarlar. Birim EMU. |
| [XAngle](../../aspose.cells.drawing/shapepathpoint/xangle/) { get; set; } | Nesne bir açı işaretçisi olduğunda, ilk açıyı derece cinsinden alır veya ayarlar. |
| [XPixel](../../aspose.cells.drawing/shapepathpoint/xpixel/) { get; set; } | Nesne bir konum koordinatı olduğunda, x koordinatını piksel cinsinden alır veya ayarlar. |
| [Y](../../aspose.cells.drawing/shapepathpoint/y/) { get; set; } | (**Obsolete.**) Bu konum koordinatı için y koordinatını alır. Birim EMU. |
| [YAngle](../../aspose.cells.drawing/shapepathpoint/yangle/) { get; set; } | Nesne bir açı işaretçisi olduğunda, ikinci açıyı derece cinsinden alır veya ayarlar. |
| [YPixel](../../aspose.cells.drawing/shapepathpoint/ypixel/) { get; set; } | Nesne bir konum koordinatı olduğunda, y koordinatını piksel cinsinden alır veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Gerekli tüm parametrelerle yol noktalarını içerecek bir şekil ekle.
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 10, 10, 200, 200);
                
                // Geometri yol noktalarını al.
                CustomGeometry geometry = shape.Geometry as CustomGeometry;
                if (geometry != null && geometry.Paths.Count > 0)
                {
                    ShapePath path = geometry.Paths[0];
                    
                    // Mevcut bir yol noktasına eriş (varsa).
                    if (path.PathSegementList.Count > 0)
                    {
                        // İlk noktayı al (gerçek uygulama segment tipine göre değişebilir).
                        ShapePathPoint point = path.PathSegementList[0].Points[0];
                        
                        // Nokta koordinatlarını göster
                        Console.WriteLine($"ShapePathPoint at X: {point.X}, Y: {point.Y}");
                    }
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ShapePathPointDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPoint: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


