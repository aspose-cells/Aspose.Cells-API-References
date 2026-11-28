---
title: "ShapePath sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ShapePath sınıfı. Bir dizi hareket, çizgi ve eğriden oluşan ve birleştirildiğinde geometrik bir şekil oluşturan bir oluşturma yolunu temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shapepath/
---
## ShapePath class

Bir dizi hareket, çizgi ve eğriden oluşan ve birleştirildiğinde geometrik bir şekil oluşturacak bir oluşturma yolunu temsil eder.

```csharp
public class ShapePath
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ShapePath](shapepath/)() | `ShapePath` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [HeightPixel](../../aspose.cells.drawing/shapepath/heightpixel/) { get; set; } | Bu yolun yüksekliğini piksel biriminde alır. |
| [PathSegementList](../../aspose.cells.drawing/shapepath/pathsegementlist/) { get; } | (**Obsolete.**) [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) listesini alır |
| [PathSegments](../../aspose.cells.drawing/shapepath/pathsegments/) { get; } | [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) listesini alır |
| [WidthPixel](../../aspose.cells.drawing/shapepath/widthpixel/) { get; set; } | Bu yolun genişliğini piksel biriminde alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ArcTo](../../aspose.cells.drawing/shapepath/arcto/)(float, float, float, float) | Mevcut şekle eliptik bir yay ekler. Başlangıç noktası, mevcut şeklin son noktasıdır. |
| [Close](../../aspose.cells.drawing/shapepath/close/)() | Mevcut şekli kapatır ve yeni bir şekil başlatır. Mevcut şekil bağlı çizgiler ve eğrilerden oluşan bir dizi içeriyorsa, yöntem son noktayı başlangıç noktasına bir çizgiyle bağlayarak döngüyü kapatır. |
| [CubicBezierTo](../../aspose.cells.drawing/shapepath/cubicbezierto/)(float, float, float, float, float, float) | Mevcut şekle kübik Bézier eğrisi ekler. Başlangıç noktası, mevcut şeklin son noktasıdır. Unit: Pixel. |
| [LineTo](../../aspose.cells.drawing/shapepath/lineto/)(float, float) | Mevcut şekle bir çizgi segmenti ekler. Başlangıç noktası, mevcut şeklin son noktasıdır. Unit: Pixel. |
| [MoveTo](../../aspose.cells.drawing/shapepath/moveto/)(float, float) | Belirtilen noktadan mevcut şekli kapatmadan yeni bir şekil başlatır. Yola eklenen sonraki tüm noktalar bu yeni şekle eklenir. Unit: Pixel. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePathDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tüm gerekli parametrelerle özel bir şekil ekle
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            
            // ShapePathCollection'a erişin
            ShapePathCollection shapePaths = customShape.Paths;

            // Yeni bir yol ekle ve ona eriş
            int pathIndex = shapePaths.Add();
            ShapePath newPath = shapePaths[pathIndex];

            // Yolların sayısını çıktı olarak göster
            Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count.ToString());

            // Çalışma kitabını kaydedin
            workbook.Save("ShapePathDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


