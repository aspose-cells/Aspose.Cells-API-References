---
title: "MsoLineFormat.Style"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoLineFormat özelliği. Belirtilen aralığın stilini temsil eden bir Style nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/msolineformat/style/
---
## MsoLineFormat.Style property

Belirtilen aralığın stilini temsil eden bir Style nesnesi döndürür.

```csharp
public MsoLineStyle Style { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekleyin
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 10, 10);

            // Çizgi biçimini alın
            MsoLineFormat lineFormat = line.LineFormat;

            // Satır stil özelliklerini ayarla
            lineFormat.Style = MsoLineStyle.ThickBetweenThin;
            lineFormat.ForeColor = System.Drawing.Color.Red;
            lineFormat.BackColor = System.Drawing.Color.White;
            lineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 3.0;

            // Karşılaştırma için başka bir satır oluştur
            Aspose.Cells.Drawing.LineShape line2 = worksheet.Shapes.AddLine(5, 25, 100, 150, 10, 10);
            MsoLineFormat lineFormat2 = line2.LineFormat;

            // Stili ilk satırdan ikinci satıra kopyala
            lineFormat2.Style = lineFormat.Style;
            lineFormat2.ForeColor = lineFormat.ForeColor;
            lineFormat2.BackColor = lineFormat.BackColor;
            lineFormat2.DashStyle = lineFormat.DashStyle;
            lineFormat2.Transparency = lineFormat.Transparency;
            lineFormat2.Weight = lineFormat.Weight;

            // Çalışma kitabını kaydedin
            workbook.Save("MsoLineFormatStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


