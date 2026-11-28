---
title: "TextParagraph.DefaultTabSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraph özelliği. Bu paragraftaki sekme karakteri için varsayılan boyutu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/defaulttabsize/
---
## TextParagraph.DefaultTabSize property

Bu paragraftaki sekme karakteri için varsayılan boyutu alır ve ayarlar.

```csharp
public double DefaultTabSize { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyDefaultTabSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 200);
            textBox.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Metin kutusunun ilk paragrafından metin paragrafını alın
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Mevcut varsayılan sekme boyutunu göster
            Console.WriteLine("Current DefaultTabSize: " + paragraph.DefaultTabSize);

            // Daha küçük bir sekme boyutu ayarlayın (varsayılan genellikle yaklaşık 36 puandır)
            paragraph.DefaultTabSize = 20.0;
            Console.WriteLine("DefaultTabSize set to: " + paragraph.DefaultTabSize);

            // Karşılaştırma için varsayılan sekme boyutlu başka bir metin kutusu ekleyin
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 3, 1, 3, 300, 200);
            textBox2.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Sekme aralığındaki farkı görmek için çalışma kitabını kaydedin
            workbook.Save("TextParagraphDefaultTabSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


