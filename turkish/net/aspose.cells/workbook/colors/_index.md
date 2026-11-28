---
title: "Workbook.Colors"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Elektronik tablo için palet içindeki renkleri döndürür"
type: docs
url: /tr/net/aspose.cells/workbook/colors/
---
## Workbook.Colors property

Elektronik tablo için palet içindeki renkleri döndürür.

```csharp
public Color[] Colors { get; }
```

### Açıklamalar

Palet 56 girdi içerir, her biri bir RGB değeriyle temsil edilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyColorsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Varsayılan renk paletine eriş
            Color[] colors = workbook.Colors;

            // Palet içindeki bazı renkleri değiştir
            colors[0] = System.Drawing.Color.Red;      // Modify first color to Red
            colors[1] = System.Drawing.Color.Green;    // Modify second color to Green
            colors[2] = System.Drawing.Color.Blue;    // Modify third color to Blue

            // Bir çalışma sayfası oluşturun ve bazı veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Color Demo");
            
            // Değiştirilen renkleri hücrelere uygula
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = colors[0];
            style1.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = colors[1];
            style2.Pattern = BackgroundType.Solid;
            worksheet.Cells["B2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = colors[2];
            style3.Pattern = BackgroundType.Solid;
            worksheet.Cells["C2"].SetStyle(style3);

            // Çalışma kitabını kaydedin
            workbook.Save("WorkbookColorsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


