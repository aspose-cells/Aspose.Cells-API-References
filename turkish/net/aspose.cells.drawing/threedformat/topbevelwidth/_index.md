---
title: "ThreeDFormat.TopBevelWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. Üst köşebentinin genişliğini veya şekle ne kadar uygulandığını alır ve ayarlar. Birim olarak Nokta"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/topbevelwidth/
---
## ThreeDFormat.TopBevelWidth property

Üst köşebentinin genişliğini alır ve ayarlar, ya da şekle ne kadar uygulandığını. Birim olarak Puan.

```csharp
public double TopBevelWidth { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına doğru parametrelerle bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 0, 0);

            // Şeklin 3D biçimini al
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // TopBevelWidth dahil olmak üzere 3D özelliklerini ayarla
            threeDFormat.TopBevelType = BevelType.HardEdge;
            threeDFormat.TopBevelWidth = 30;
            threeDFormat.TopBevelHeight = 30;
            threeDFormat.ContourWidth = 17;
            threeDFormat.ExtrusionHeight = 32;

            // Çalışma kitabını kaydedin
            workbook.Save("ThreeDFormatDemo.xlsx");

            // Kaydedilen özellikleri doğrula
            Workbook loadedWorkbook = new Workbook("ThreeDFormatDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;

            Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
            Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
            Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
            Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
            Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


