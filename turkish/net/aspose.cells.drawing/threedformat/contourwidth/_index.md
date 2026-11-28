---
title: "ThreeDFormat.ContourWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreeDFormat özelliği. Şekilde kontur genişliğini birim olarak nokta cinsinden alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/threedformat/contourwidth/
---
## ThreeDFormat.ContourWidth property

Şeklin kontur genişliğini alır ve ayarlar, birim: nokta.

```csharp
public double ContourWidth { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyContourWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Gerekli tüm parametrelerle çalışma sayfasına bir şekil ekle
            Shape sh = ws.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);

            // 3D biçimlendirmeyi uygula
            ThreeDFormat n3df = sh.ThreeDFormat;
            n3df.ContourWidth = 17;
            n3df.ExtrusionHeight = 32;
            n3df.TopBevelType = (BevelType)BevelPresetType.HardEdge;

            // Çalışma kitabını kaydedin
            wb.Save("output.xlsx");

            // Kaydedilen değerleri doğrula
            Workbook wb2 = new Workbook("output.xlsx");
            Shape sh2 = wb2.Worksheets[0].Shapes[0];
            ThreeDFormat n3df2 = sh2.ThreeDFormat;

            Console.WriteLine("ContourWidth: " + n3df2.ContourWidth);
            Console.WriteLine("ExtrusionHeight: " + n3df2.ExtrusionHeight);
            Console.WriteLine("TopBevelType: " + n3df2.TopBevelType);
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


