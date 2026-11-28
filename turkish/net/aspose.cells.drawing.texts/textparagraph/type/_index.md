---
title: "TextParagraph.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraph özelliği. Metin düğümünün tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/type/
---
## TextParagraph.Type property

Metin düğümünün tipini alır.

```csharp
public override TextNodeType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına tüm gerekli parametrelerle bir metin kutusu ekle
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            var textBody = textBox.TextBody;
            textBody.Text = "Sample Text\nSecond Line";

            // Metin gövdesinden ilk paragrafı al
            var paragraphs = textBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[0];

            // Mevcut Type değerini göster
            Console.WriteLine("Current TextNodeType: " + paragraph.Type);

            // Type özelliğinin davranışı nasıl etkilediğini göster
            if (paragraph.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("This is a text paragraph node");
                Console.WriteLine("You can access paragraph-specific properties like:");
                Console.WriteLine("AlignmentType: " + paragraph.AlignmentType);
                Console.WriteLine("LineSpace: " + paragraph.LineSpace);
            }
            else if (paragraph.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("This is a simple text run node");
            }
            else if (paragraph.Type == TextNodeType.Equation)
            {
                Console.WriteLine("This is an equation node");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("TextParagraphPropertyTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextNodeType](../../textnodetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


