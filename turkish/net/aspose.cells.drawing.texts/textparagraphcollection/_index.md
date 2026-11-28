---
title: "Sınıf TextParagraphCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.TextParagraphCollection sınıfı. Tüm metin paragraflarını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraphcollection/
---
## TextParagraphCollection class

Tüm metin paragrafının temsilidir.

```csharp
public class TextParagraphCollection : IEnumerable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.cells.drawing.texts/textparagraphcollection/count/) { get; } | Metin paragraflarının sayısını alır. |
| [Item](../../aspose.cells.drawing.texts/textparagraphcollection/item/) { get; } | Belirli indeksteki [`TextParagraph`](../textparagraph/) nesnesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetEnumerator](../../aspose.cells.drawing.texts/textparagraphcollection/getenumerator/)() | Paragrafların enumerator'ını alır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphCollectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bir metin kutusu ekle
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            
            // Çok satırlı metni ayarla
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Paragraf koleksiyonunu al
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // İkinci paragrafı eriş ve değiştir
            TextParagraph secondParagraph = paragraphs[1];
            secondParagraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            secondParagraph.LineSpace = 20;
            secondParagraph.SpaceAfter = 30;
            secondParagraph.SpaceBefore = 40;
            
            // Çalışma kitabını kaydedin
            workbook.Save("TextParagraphCollectionDemo.xlsx");
            
            Console.WriteLine("Text paragraph formatting saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


