---
title: "TextParagraph.FontAlignType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraph özelliği. Metin satırındaki gerçek kelimelerin dikey olarak nerede konumlandırıldığını belirler. Bu, karakterlerin temel çizgilere göre dikey yerleşimini ele alır"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/fontaligntype/
---
## TextParagraph.FontAlignType property

Metin satırında kelimelerin dikey olarak nerede konumlandırıldığını belirler. Bu, karakterlerin temel çizgilere göre dikey yerleşimini kapsar.

```csharp
public TextFontAlignType FontAlignType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFontAlignTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            int textboxIndex = worksheet.TextBoxes.Add(1, 1, 200, 400);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample Text\nFor Font Alignment Demo";

            // Metin kutusunun ilk paragrafını alın
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];

            // Mevcut FontAlignType değerini göster
            Console.WriteLine("Current FontAlignType value: " + paragraph.FontAlignType);

            // FontAlignType'ı Alt olarak ayarlayın
            paragraph.FontAlignType = TextFontAlignType.Bottom;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // FontAlignType'ı Ortaya ayarlayın
            paragraph.FontAlignType = TextFontAlignType.Center;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // FontAlignType'ı Üst olarak ayarlayın
            paragraph.FontAlignType = TextFontAlignType.Top;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Etkileri görmek için çalışma kitabını kaydedin
            workbook.Save("TextParagraphPropertyFontAlignTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextFontAlignType](../../textfontaligntype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


