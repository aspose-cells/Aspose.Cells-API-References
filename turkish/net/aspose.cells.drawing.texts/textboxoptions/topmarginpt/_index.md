---
title: "TextBoxOptions.TopMarginPt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxOptions özelliği. Üst kenar boşluğunu puan biriminde alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textboxoptions/topmarginpt/
---
## TextBoxOptions.TopMarginPt property

Üst kenar boşluğunu Nokta biriminde alır ve ayarlar.

```csharp
public double TopMarginPt { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir metin kutusu ekle
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Üst kenar boşluğunu puan cinsinden ayarla
            textBox.TextBoxOptions.TopMarginPt = 0.2d;
            
            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxTopMarginDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


