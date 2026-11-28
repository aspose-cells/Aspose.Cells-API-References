---
title: "Enum TextOverflowType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.TextOverflowType enum. Metnin dikey veya yatay taşma şeklini temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing/textoverflowtype/
---
## TextOverflowType enumeration

Metnin dikey veya yatay taşma şeklini temsil eder.

```csharp
public enum TextOverflowType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Clip | `0` | Üst ve alt engellere dikkat edin. Görünmeyen bir metin olduğuna dair hiçbir gösterge vermeyin. |
| Ellipsis | `1` | Üst ve alt engellere dikkat edin. Görünmeyen bir metni göstermek için üç nokta kullanın. Yalnızca dikey taşma için. |
| Overflow | `2` | Metni taşırın ve üst ile alt engellere dikkat etmeyin. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassTextOverflowTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe bir metin kutusu ekleyin.
            TextBox textBox = chart.Shapes.AddTextBoxInChart(10, 10, 200, 50);

            // Metin kutusu özelliklerini ayarlayın.
            textBox.TextBody.TextAlignment.AutoSize = false;
            textBox.Text = "This is a long text that will demonstrate text overflow handling";
            
            // Metin taşma tipini ayarlayın.
            textBox.TextVerticalOverflow = TextOverflowType.Clip;

            // Çalışma kitabını kaydedin
            workbook.Save("TextOverflowTypeDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


