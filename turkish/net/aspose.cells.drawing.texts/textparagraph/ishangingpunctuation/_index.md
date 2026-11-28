---
title: "TextParagraph.IsHangingPunctuation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraph özelliği. Noktalama işaretlerinin metin satırına zorla yerleştirilip yerleştirilmeyeceğini veya farklı bir satıra konulup konulmayacağını belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/
---
## TextParagraph.IsHangingPunctuation property

Noktalama işaretlerinin metin satırına zorla yerleştirilip yerleştirilmeyeceğini veya farklı bir satıra konulup konulmayacağını belirtir.

```csharp
public bool IsHangingPunctuation { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsHangingPunctuationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekleyin (yükseklik parametresi eklenerek düzeltildi)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 100, 200, 100);
            textBox.Text = "This is a sample text with punctuation: \"Hello, world!\"";

            // Metin kutusundan metin paragrafını alın (TextParagraph tipine dönüştürülerek düzeltildi)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // IsHangingPunctuation değerinin mevcut durumunu göster
            Console.WriteLine("Current IsHangingPunctuation value: " + textParagraph.IsHangingPunctuation);

            // IsHangingPunctuation değerini true olarak ayarlayın
            textParagraph.IsHangingPunctuation = true;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // IsHangingPunctuation değerini false olarak ayarlayın
            textParagraph.IsHangingPunctuation = false;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // Etkileri görmek için çalışma kitabını kaydedin (görsel inceleme gerekir)
            workbook.Save("TextParagraphPropertyIsHangingPunctuationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


