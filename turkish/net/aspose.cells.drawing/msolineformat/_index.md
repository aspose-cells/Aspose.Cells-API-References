---
title: "Class MsoLineFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MsoLineFormat sınıfı. Çizgi ve ok ucu biçimlendirmesini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/msolineformat/
---
## MsoLineFormat class

Çizgi ve ok ucu biçimlendirmesini temsil eder.

```csharp
public class MsoLineFormat
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformat/backcolor/) { get; set; } | Kenarlık çizgi arka plan rengini alır ve ayarlar. |
| [DashStyle](../../aspose.cells.drawing/msolineformat/dashstyle/) { get; set; } | Belirtilen çizgi için kesikli stilini alır veya ayarlar. |
| [ForeColor](../../aspose.cells.drawing/msolineformat/forecolor/) { get; set; } | Kenarlık çizgi ön plan rengini alır ve ayarlar. |
| [IsVisible](../../aspose.cells.drawing/msolineformat/isvisible/) { get; set; } | Nesnenin görünür olup olmadığını gösterir. |
| [Style](../../aspose.cells.drawing/msolineformat/style/) { get; set; } | Belirtilen aralığın stilini temsil eden bir Style nesnesi döndürür. |
| [Transparency](../../aspose.cells.drawing/msolineformat/transparency/) { get; set; } | Belirtilen dolgunun şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [Weight](../../aspose.cells.drawing/msolineformat/weight/) { get; set; } | Çizginin kalınlığını puan (pt) biriminde döndürür veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatDemo
    {
        public static void MsoLineFormatExample()
        {
            // Yeni bir Workbook örneği oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir yay şekli ekleyin
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Şekilden MsoLineFormat nesnesini alın
            MsoLineFormat lineFormat = arcShape.LineFormat;

            // MsoLineFormat nesnesinin özelliklerini ayarlayın
            lineFormat.IsVisible = true;
            lineFormat.Style = MsoLineStyle.ThickThin;
            lineFormat.ForeColor = Color.Red;
            lineFormat.BackColor = Color.Blue;
            lineFormat.DashStyle = MsoLineDashStyle.Solid;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 2.0;

            // Çalışma kitabını kaydedin
            workbook.Save("MsoLineFormatExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


