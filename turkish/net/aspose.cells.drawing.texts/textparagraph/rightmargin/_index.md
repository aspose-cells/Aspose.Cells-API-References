---
title: "TextParagraph.RightMargin"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraph özelliği. Paragrafın sağ kenar boşluğunu belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/rightmargin/
---
## TextParagraph.RightMargin property

Paragrafın sağ kenar boşluğunu belirtir.

```csharp
public double RightMargin { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "This is a sample text to demonstrate RightMargin property of TextParagraph.";

            // Metin kutusunun ilk paragrafından metin paragrafını alın
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Mevcut sağ kenar boşluğu değerini göster
            Console.WriteLine("Current RightMargin value: " + paragraph.RightMargin);

            // Yeni bir sağ kenar boşluğu değeri ayarlayın (puan cinsinden)
            paragraph.RightMargin = 20.0;

            // Farkı göstermek için başka bir metin kutusu ekleyin
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 2, 1, 2, 200, 200);
            textBox2.Text = "This text has default RightMargin for comparison.";
            
            // Etkiyi görmek için çalışma kitabını kaydet
            workbook.Save("TextParagraphRightMarginDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


