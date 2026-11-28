---
title: "Sınıf MsoFillFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MsoFillFormat sınıfı. Bir şekil için dolgu biçimlendirmesini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/msofillformat/
---
## MsoFillFormat class

Bir şekil için dolgu biçimlendirmesini temsil eder.

```csharp
public class MsoFillFormat
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformat/backcolor/) { get; set; } | Dosyanın arka rengini alır ve ayarlar. |
| [ForeColor](../../aspose.cells.drawing/msofillformat/forecolor/) { get; set; } | Doldurma ön rengini alır ve ayarlar. |
| [ImageData](../../aspose.cells.drawing/msofillformat/imagedata/) { get; set; } | Doku ve Resim dolgu verilerini alır ve ayarlar. |
| [IsVisible](../../aspose.cells.drawing/msofillformat/isvisible/) { get; set; } | Dolgu olup olmadığını gösterir. |
| [Texture](../../aspose.cells.drawing/msofillformat/texture/) { get; } | Doku dolgu tipini alır. |
| [Transparency](../../aspose.cells.drawing/msofillformat/transparency/) { get; set; } | Belirtilen dolgunun şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Belirtilen dolguyu tek renkli bir degrade olarak ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatDemo
    {
        public static void MsoFillFormatExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir yay şekli ekleyin
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Şeklin dolgu biçimine erişin
            MsoFillFormat fillFormat = arcShape.FillFormat;

            // Dolgu ön rengini ayarlayın
            fillFormat.ForeColor = Color.Blue;

            // Dolgu arka rengini ayarlayın
            fillFormat.BackColor = Color.LightBlue;

            // Şeffaflığı ayarlayın
            fillFormat.Transparency = 0.5;

            // Dolgunun görünür olup olmadığını kontrol edin
            bool isVisible = fillFormat.IsVisible;
            Console.WriteLine("Is Fill Visible: " + isVisible);

            // Tek renkli bir degrade dolgu ayarlayın
            fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);

            // Çalışma kitabını kaydedin
            workbook.Save("MsoFillFormatExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


