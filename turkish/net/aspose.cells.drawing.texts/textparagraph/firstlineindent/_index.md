---
title: "TextParagraph.FirstLineIndent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraph özelliği. Paragraftaki ilk satır metnine uygulanacak girinti boyutunu belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/firstlineindent/
---
## TextParagraph.FirstLineIndent property

Paragraftaki metnin ilk satırına uygulanacak girinti boyutunu belirtir.

```csharp
public double FirstLineIndent { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFirstLineIndentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 100, 300, 200, 100);
            textBox.Text = "This is a sample paragraph with multiple lines.\nFirst line should have indent.\nSecond line should be normal.";

            // Metin kutusundan metin paragrafını alın
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Mevcut FirstLineIndent değerini göster
            Console.WriteLine("Current FirstLineIndent value: " + textParagraph.FirstLineIndent);

            // Yeni bir FirstLineIndent değeri ayarlayın (20 puan)
            textParagraph.FirstLineIndent = 20;
            Console.WriteLine("FirstLineIndent set to: " + textParagraph.FirstLineIndent);

            // Varsayılan girinti ile karşılaştırmak için başka bir metin kutusu ekleyin
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 5, 150, 300, 200, 100);
            textBox2.Text = "This is a comparison paragraph without indent.\nFirst line has no indent.\nSecond line is normal.";

            // Etkileri görmek için çalışma kitabını kaydedin
            workbook.Save("TextParagraphPropertyFirstLineIndentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


