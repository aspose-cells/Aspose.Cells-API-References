---
title: "FontSettingCollection.TextParagraphs"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSettingCollection özelliği. Tüm paragrafları alır"
type: docs
url: /tr/net/aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/
---
## FontSettingCollection.TextParagraphs property

Tüm paragrafları alır.

```csharp
public TextParagraphCollection TextParagraphs { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyTextParagraphsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "First paragraph\nSecond paragraph";

            // İlk metin paragrafına erişin
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            
            // Satır aralığı özelliklerini ayarlayın
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000; // 300% line spacing

            // Madde işareti özelliklerini ayarlayın
            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Çalışma kitabını kaydedin
            workbook.Save("TextParagraphsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextParagraphCollection](../../textparagraphcollection/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


