---
title: "TextBoxOptions.RightMarginPt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxOptions özelliği. Sağ kenar boşluğunu puan biriminde alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textboxoptions/rightmarginpt/
---
## TextBoxOptions.RightMarginPt property

Sağ kenar boşluğunu Nokta biriminde alır ve ayarlar.

```csharp
public double RightMarginPt { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyRightMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            int textBoxIndex = worksheet.TextBoxes.Add(1, 1, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "Sample Text";

            // Sağ kenar boşluğunu puan cinsinden ayarla
            textBox.TextBoxOptions.RightMarginPt = 0.2d;

            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxRightMarginDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


