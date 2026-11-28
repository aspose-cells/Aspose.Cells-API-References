---
title: "Style.RotationAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Metin döndürme açısını temsil eder"
type: docs
url: /tr/net/aspose.cells/style/rotationangle/
---
## Style.RotationAngle property

Metin döndürme açısını temsil eder.

```csharp
public int RotationAngle { get; set; }
```

### Açıklamalar

0: Döndürülmedi.

255: Üstten Alta.

-90: Downward.

90: Yukarı.

255 veya -90 ile 90 arasında bir değer ayarlayabilirsiniz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Farklı döndürme açılarıyla bir stil oluşturun
            Style style1 = workbook.CreateStyle();
            style1.RotationAngle = -90;
            worksheet.Cells["B2"].PutValue("Text rotated -90°");
            worksheet.Cells["B2"].SetStyle(style1);

            Style style2 = workbook.CreateStyle();
            style2.RotationAngle = 90;
            worksheet.Cells["C3"].PutValue("Text rotated 90°");
            worksheet.Cells["C3"].SetStyle(style2);

            Style style3 = workbook.CreateStyle();
            style3.RotationAngle = 255;
            worksheet.Cells["D4"].PutValue("Text rotated 255°");
            worksheet.Cells["D4"].SetStyle(style3);

            // Çalışma kitabını kaydedin
            workbook.Save("output_rotation_angles.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


