---
title: "Enum LineSpaceSizeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.LineSpaceSizeType enum. Satır aralığı boyutunun birim türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/linespacesizetype/
---
## LineSpaceSizeType enumeration

Satır aralığı boyutunun birim türünü temsil eder.

```csharp
public enum LineSpaceSizeType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Percentage | `0` | Metin boyutunun yüzde birimi olarak temsil eder. |
| Points | `1` | Nokta biriminde temsil eder. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir metin kutusu şekli ekle
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Metin içeriğini ayarla
            textBox.Text = "Sample Text\nSecond Line";
            
            // Metin kutusunun ilk paragrafına eriş
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
            
            // Sonraki boşluk boyut türünü Nokta olarak ayarla
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            // Sonraki boşluk değerini ayarla (12 nokta)
            paragraph.SpaceAfter = 12;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Text box with line spacing created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


