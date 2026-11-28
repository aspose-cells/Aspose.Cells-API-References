---
title: "Style.HorizontalAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Bir hücredeki metnin yatay hizalama türünü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/style/horizontalalignment/
---
## Style.HorizontalAlignment property

Bir hücredeki metnin yatay hizalama türünü alır veya ayarlar.

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücrelere metin ayarla
            cells["A1"].PutValue("Left Aligned");
            cells["A2"].PutValue("Center Aligned");
            cells["A3"].PutValue("Right Aligned");

            // Stil nesnelerini al
            Style styleLeft = cells["A1"].GetStyle();
            Style styleCenter = cells["A2"].GetStyle();
            Style styleRight = cells["A3"].GetStyle();

            // Yatay hizalamayı ayarla
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            styleRight.HorizontalAlignment = TextAlignmentType.Right;

            // Stilleri hücrelere uygula
            cells["A1"].SetStyle(styleLeft);
            cells["A2"].SetStyle(styleCenter);
            cells["A3"].SetStyle(styleRight);

            // Çalışma kitabını kaydedin
            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


