---
title: "TextParagraph.IsLatinLineBreak"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraph özelliği. Bir Latin kelimesinin yarıya bölünüp tire eklenmeden bir sonraki satıra taşınıp taşınamayacağını belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/islatinlinebreak/
---
## TextParagraph.IsLatinLineBreak property

Bir Latin kelimesinin ikiye bölünüp tire eklenmeden bir sonraki satıra kaydırılıp kaydırılamayacağını belirtir.

```csharp
public bool IsLatinLineBreak { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsLatinLineBreakDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekleyin (yükseklik dahil edilmek üzere sabit parametreler)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "This is a long Latin text that will demonstrate line breaking behavior when IsLatinLineBreak is set to different values.";

            // Metin kutusunun metin paragrafını alın (açık dönüşüm eklendi)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = ((TextParagraph)fontSetting);

            // IsLatinLineBreak değerinin mevcut durumunu göster
            Console.WriteLine("Current IsLatinLineBreak value: " + textParagraph.IsLatinLineBreak);

            // IsLatinLineBreak değerini false olarak ayarlayın (Latin kelimeleri satır sonunda bölünmez)
            textParagraph.IsLatinLineBreak = false;
            Console.WriteLine("Set IsLatinLineBreak to false - Latin words won't break at line end");
            workbook.Save("LatinLineBreakDisabled.xlsx");

            // IsLatinLineBreak değerini true olarak ayarlayın (Latin kelimeleri satır sonunda bölünebilir)
            textParagraph.IsLatinLineBreak = true;
            Console.WriteLine("Set IsLatinLineBreak to true - Latin words can break at line end");
            workbook.Save("LatinLineBreakEnabled.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


