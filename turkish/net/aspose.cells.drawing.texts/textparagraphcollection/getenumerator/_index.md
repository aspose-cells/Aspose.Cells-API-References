---
title: "TextParagraphCollection.GetEnumerator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextParagraphCollection yöntemi. Paragrafların enumerator'ünü alır"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textparagraphcollection/getenumerator/
---
## TextParagraphCollection.GetEnumerator method

Paragrafların enumerator'ını alır.

```csharp
public IEnumerator GetEnumerator()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.Collections;

    public class TextParagraphCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına tüm gerekli parametrelerle bir metin kutusu ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 200, 100, 100);
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Metin paragrafı koleksiyonunu al
            TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;

            try
            {
                // GetEnumerator yöntemini çağırın
                IEnumerator enumerator = paragraphs.GetEnumerator();

                Console.WriteLine($"Number of paragraphs: {paragraphs.Count}");
                Console.WriteLine("Paragraphs:");

                // Paragraflar üzerinde yineleyici kullanarak dolaş
                while (enumerator.MoveNext())
                {
                    TextParagraph paragraph = (TextParagraph)enumerator.Current;
                    Console.WriteLine(textBox.Text); // Using the text from the textbox since TextParagraph doesn't have Text property
                }

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("MethodGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


