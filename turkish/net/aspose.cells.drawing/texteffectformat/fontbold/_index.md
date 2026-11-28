---
title: "TextEffectFormat.FontBold"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextEffectFormat özelliği. Yazı tipinin kalın olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/texteffectformat/fontbold/
---
## TextEffectFormat.FontBold property

Yazı tipinin kalın olup olmadığını gösterir.

```csharp
public bool FontBold { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir metin kutusu şekli ekle (TextBox nesnesini doğrudan döndürür)
            TextBox textbox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
            textbox.Text = "Sample Text";

            // Metin efekti formatını al
            TextEffectFormat effFormat = textbox.TextEffect;

            // Kalın dahil olmak üzere yazı tipi özelliklerini ayarla
            effFormat.FontName = "Arial";
            effFormat.FontBold = true;
            effFormat.FontItalic = false;
            effFormat.FontSize = 14;

            // Çalışma kitabını kaydedin
            workbook.Save("TextEffectFormatFontBoldDemo.xlsx");

            Console.WriteLine("Text effect format with bold font applied successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


