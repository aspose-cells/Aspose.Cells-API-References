---
title: "TextParagraph.LeftMargin"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraph özelliği. Paragrafın sol kenar boşluğunu belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/leftmargin/
---
## TextParagraph.LeftMargin property

Paragrafın sol kenar boşluğunu belirtir.

```csharp
public double LeftMargin { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 2, 200, 200);
            textBox.Text = "This is a sample text paragraph.\nSecond line of the paragraph.";

            // Metin kutusunun ilk paragrafından metin paragrafını alın
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Mevcut sol kenar boşluğu değerini göster
            Console.WriteLine("Current LeftMargin value: " + paragraph.LeftMargin);

            // Yeni bir sol kenar boşluğu değeri ayarlayın (puan cinsinden)
            paragraph.LeftMargin = 20.0;

            // Varsayılan kenar boşluğu ile başka bir metin kutusu ekleyerek etkiyi gösterin
            TextBox textBox2 = worksheet.Shapes.AddTextBox(0, 3, 2, 2, 200, 200);
            textBox2.Text = "This text box has default left margin.\nCompare the indentation.";

            // Farkı göstermek için çalışma kitabını kaydedin
            workbook.Save("TextParagraphLeftMarginDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


