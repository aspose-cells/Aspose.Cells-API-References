---
title: "TextParagraph.Children"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraph özelliği. Bu paragraftaki tüm metin akışlarını alır. Eğer bu paragraf boşsa paragrafı kendisini döndürür"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/children/
---
## TextParagraph.Children property

Bu paragraftaki tüm metin akışlarını alır. Bu paragraf boşsa, paragrafı kendisini döndürür.

```csharp
public FontSetting[] Children { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyChildrenDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 100, 200);
            textBox.Text = "First line\nSecond line\nThird line";

            // Metin paragrafı koleksiyonunu al
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Paragraftaki alt öğelerin (metin akışları) sayısını göster
            Console.WriteLine("Number of children (text runs): " + textParagraph.Children.Length);

            // Her alt öğenin (metin akışı) yazı tipi ayarlarını değiştir
            foreach (FontSetting child in textParagraph.Children)
            {
                child.Font.Size = 12;
                child.Font.Color = System.Drawing.Color.Blue;
                child.Font.IsBold = true;
            }

            // Farklı biçimlendirme ile başka bir satır ekle
            textBox.Text += "\nFourth line";
            fontSetting = (FontSetting)textBox.GetCharacters()[textBox.Text.Length - 1];
            textParagraph = (TextParagraph)fontSetting;

            // Güncellenmiş çocuk sayısını göster
            Console.WriteLine("Updated number of children: " + textParagraph.Children.Length);

            // Çalışma kitabını kaydedin
            workbook.Save("TextParagraphChildrenDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


