---
title: "Sınıf ColorHelper"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ColorHelper sınıfı. Renk hakkında yardımcı işlevler sağlar"
type: docs
url: /tr/net/aspose.cells.drawing/colorhelper/
---
## ColorHelper class

Renk ile ilgili yardımcı işlevler sağlar.

```csharp
public class ColorHelper
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [FromOleColor](../../aspose.cells.drawing/colorhelper/fromolecolor/)(int) | OLE_COLOR dönüştür. |
| static [ToOleColor](../../aspose.cells.drawing/colorhelper/toolecolor/)(Color, Workbook) | Rengi OLE_COLOR'a dönüştür |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassColorHelperDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // OLE rengini System.Drawing.Color (Yeşil) olarak dönüştür
            int oleGreen = 0x00FF00;
            Color colorFromOle = ColorHelper.FromOleColor(oleGreen);

            // Dönüştürülmüş rengi A1 hücresinin arka planına uygula
            Cell cellA1 = worksheet.Cells["A1"];
            Style styleA1 = cellA1.GetStyle();
            styleA1.ForegroundColor = colorFromOle;
            styleA1.Pattern = BackgroundType.Solid;
            cellA1.SetStyle(styleA1);

            // System.Drawing.Color'ı OLE rengine geri dönüştür
            int convertedOle = ColorHelper.ToOleColor(colorFromOle, workbook);

            // OLE sonucunu Color'a geri dönüştür (doğrulama)
            Color colorFromConvertedOle = ColorHelper.FromOleColor(convertedOle);

            // Yeniden dönüştürülmüş rengi A2 hücresinin arka planına uygula
            Cell cellA2 = worksheet.Cells["A2"];
            Style styleA2 = cellA2.GetStyle();
            styleA2.ForegroundColor = colorFromConvertedOle;
            styleA2.Pattern = BackgroundType.Solid;
            cellA2.SetStyle(styleA2);

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("DrawingClassColorHelperDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


