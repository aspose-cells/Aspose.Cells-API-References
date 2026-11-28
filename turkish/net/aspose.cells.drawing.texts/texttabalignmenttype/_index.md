---
title: "Enum TextTabAlignmentType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.TextTabAlignmentType enum. Metin sekme hizalama türlerini temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing.texts/texttabalignmenttype/
---
## TextTabAlignmentType enumeration

Metin sekme hizalama türlerini temsil eder.

```csharp
public enum TextTabAlignmentType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Center | `0` | Bu sekme konumundaki metin ortalanmıştır. |
| Decimal | `1` | Bu sekme konumunda ondalıklar hizalanmıştır. |
| Left | `2` | Bu sekme konumundaki metin sola hizalanmıştır. |
| Right | `3` | Bu sekme konumundaki metin sağa hizalanmıştır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextTabAlignmentTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sekme hizalamalarını göstermek için bir metin kutusu oluştur.
            int textBoxIndex = worksheet.TextBoxes.Add(0, 0, 400, 300);
            var textBox = worksheet.TextBoxes[textBoxIndex];
            var paragraph = textBox.TextBody.TextParagraphs[0];

            // Farklı hizalama türleriyle sekme durakları ekle.
            paragraph.Stops.Add(TextTabAlignmentType.Left, 100);
            paragraph.Stops.Add(TextTabAlignmentType.Center, 200);
            paragraph.Stops.Add(TextTabAlignmentType.Right, 300);
            paragraph.Stops.Add(TextTabAlignmentType.Decimal, 400);

            // Tüm hizalama türlerini göstermek için metni ayarla.
            textBox.Text = "Left\tCenter\tRight\tDecimal\n" +
                           "Data\tData\tData\t12.34\n" +
                           "More\tMore\tMore\t56.78";

            // Sekmeleri görünür kılmak için biçimlendirme uygula.
            textBox.Font.Size = 12;
            textBox.TextBody.TextParagraphs[0].AlignmentType = TextAlignmentType.Left;

            // Sonucu kaydet
            workbook.Save("TextTabAlignmentTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


