---
title: "TextEffectFormat.FontSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextEffectFormat özelliği. WordArt'ta kullanılan yazı tipinin punto cinsinden boyutu"
type: docs
url: /tr/net/aspose.cells.drawing/texteffectformat/fontsize/
---
## TextEffectFormat.FontSize property

WordArt içinde kullanılan yazı tipinin boyutu (puan cinsinden).

```csharp
public int FontSize { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            int textboxIndex = worksheet.TextBoxes.Add(5, 5, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[textboxIndex];
            
            // Metni ve biçimi ayarla
            textBox.Text = "Sample Text Effect";
            
            // Metin efekti formatını al
            Shape shape = textBox;
            TextEffectFormat effectFormat = shape.TextEffect;
            
            // FontSize dahil olmak üzere yazı tipi özelliklerini ayarla
            effectFormat.FontName = "Arial";
            effectFormat.FontBold = true;
            effectFormat.FontItalic = false;
            effectFormat.FontSize = 18; // Demonstrating FontSize property
            
            // Çalışma kitabını kaydedin
            workbook.Save("TextEffectFontSizeDemo.xlsx");
            
            Console.WriteLine("Text effect with font size 18 created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


