---
title: "TextTabStopCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextTabStopCollection yöntemi. Bir sekme durağı ekler"
type: docs
url: /tr/net/aspose.cells.drawing.texts/texttabstopcollection/add/
---
## TextTabStopCollection.Add method

Bir sekme durak ekler.

```csharp
public int Add(TextTabAlignmentType tabAlignment, double tabPosition)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tabAlignment | TextTabAlignmentType |  |
| tabPosition | Double |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopCollectionMethodAddWithTextTabAlignmentTypeDoubleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sekme duraklarıyla metin eklemek için bir şekil oluştur
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            var textParagraph = shape.TextBody.TextParagraphs[0];
            
            // TextTabStopCollection'ı al
            var tabStops = textParagraph.Stops;

            try
            {
                // TextTabAlignmentType.Left ve konum 50.0 ile Add yöntemini çağır
                int index1 = tabStops.Add(TextTabAlignmentType.Left, 50.0);
                
                // TextTabAlignmentType.Right ve konum 100.0 ile Add yöntemini çağır
                int index2 = tabStops.Add(TextTabAlignmentType.Right, 100.0);
                
                // Sekme duraklarını göstermek için sekmeli metin ekle
                shape.Text = "Left-aligned\tRight-aligned";

                Console.WriteLine("Added tab stops at positions 50.0 (Left) and 100.0 (Right)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("TextTabStopCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextTabAlignmentType](../../texttabalignmenttype/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


