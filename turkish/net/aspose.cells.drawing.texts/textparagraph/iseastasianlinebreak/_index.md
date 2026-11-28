---
title: "TextParagraph.IsEastAsianLineBreak"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraph özelliği. Bir Doğu Asya kelimesinin yarıya bölünüp tire eklenmeden bir sonraki satıra taşınıp taşınamayacağını belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/
---
## TextParagraph.IsEastAsianLineBreak property

Bir Doğu Asya kelimesinin ikiye bölünüp tire eklenmeden bir sonraki satıra kaydırılıp kaydırılamayacağını belirtir.

```csharp
public bool IsEastAsianLineBreak { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsEastAsianLineBreakDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "これは東アジアのテキストの例です。This is Latin text example.";

            // Metin kutusunun ilk paragrafından metin paragrafını alın
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // IsEastAsianLineBreak'in mevcut değerini göster
            Console.WriteLine("Current IsEastAsianLineBreak value: " + paragraph.IsEastAsianLineBreak);

            // IsEastAsianLineBreak'i false olarak ayarlayın (Doğu Asya kelimeleri bölünebilir)
            paragraph.IsEastAsianLineBreak = false;
            Console.WriteLine("After setting IsEastAsianLineBreak to false, text may break East Asian words.");

            // Doğu Asya satır sonu kesmesi devre dışı bırakılmış şekilde çalışma kitabını kaydedin
            workbook.Save("EastAsianLineBreakDisabled.xlsx");

            // IsEastAsianLineBreak'i true olarak ayarlayın (Doğu Asya kelimeleri bölünmez)
            paragraph.IsEastAsianLineBreak = true;
            Console.WriteLine("After setting IsEastAsianLineBreak to true, text won't break East Asian words.");

            // Doğu Asya satır sonu kesmesi etkinleştirilmiş şekilde çalışma kitabını kaydedin
            workbook.Save("EastAsianLineBreakEnabled.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


