---
title: "TextParagraph.Stops"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraph özelliği. Sekme durakları listesini alır"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraph/stops/
---
## TextParagraph.Stops property

Sekme durakları listesini alır.

```csharp
public TextTabStopCollection Stops { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyStopsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir hücreye metin ekleyin ve metin paragrafı özelliklerini alın
            worksheet.Cells["A1"].PutValue("Sample\tText\tWith\tTabs");
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            shape.Text = "Sample\tText\tWith\tTabs";
            
            // Metin paragrafını alın
            var textOptions = shape.TextBody.TextParagraphs[0];

            // Mevcut sekme durakları sayısını göster
            Console.WriteLine("Current tab stops count: " + textOptions.Stops.Count);

            // Yeni sekme durakları ekleyin
            textOptions.Stops.Add(TextTabAlignmentType.Left, 50);
            textOptions.Stops.Add(TextTabAlignmentType.Center, 100);
            textOptions.Stops.Add(TextTabAlignmentType.Right, 150);

            // Güncellenmiş sekme duraklarını göster
            Console.WriteLine("Updated tab stops count: " + textOptions.Stops.Count);
            for (int i = 0; i < textOptions.Stops.Count; i++)
            {
                Console.WriteLine($"Tab {i+1}: Position={textOptions.Stops[i].TabPosition}, Alignment={textOptions.Stops[i].TabAlignment}");
            }

            // Etkiyi görmek için çalışma kitabını kaydet
            workbook.Save("TextParagraphStopsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextTabStopCollection](../../texttabstopcollection/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


