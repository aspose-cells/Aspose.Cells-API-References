---
title: "Enum FillType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.FillType enum. Dolgu biçimi türü"
type: docs
url: /tr/net/aspose.cells.drawing/filltype/
---
## FillType enumeration

Dolgu biçim türü.

```csharp
public enum FillType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Automatic | `0` | Otomatik biçimlendirme türünü temsil eder. |
| None | `1` | Hiçbir biçimlendirme türünü temsil eder. |
| Solid | `2` | Katı dolgu biçimi. |
| Gradient | `3` | Gradyan doldurma biçimi. |
| Texture | `4` | Doku dolgu biçimi (resim dolgu dahil). |
| Pattern | `5` | Desen doldurma biçimi. |
| Group | `6` | Grubun dolgu özelliklerini devral. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 150);
            
            // Degrade doldurma tipini ayarlayın
            rectangle.Fill.FillType = FillType.Gradient;
            rectangle.Fill.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            // Bir metin kutusu ekle
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 10, 10, 100, 150);
            textBox.Text = "Gradient Fill Example";
            
            // Metin kutusu için degrade dolgu türünü ayarla
            textBox.Fill.FillType = FillType.Gradient;
            textBox.Fill.SetTwoColorGradient(Color.LightGreen, Color.DarkGreen, GradientStyleType.Vertical, 1);

            // Çalışma kitabını kaydedin
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


