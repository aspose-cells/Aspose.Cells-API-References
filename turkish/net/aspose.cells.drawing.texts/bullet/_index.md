---
title: "Sınıf Bullet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.Bullet sınıfı. Paragrafa uygulanması gereken madde işaretlerini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/bullet/
---
## Bullet class

Paragrafa uygulanması gereken madde işaretlerinin temsilidir.

```csharp
public class Bullet
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BulletValue](../../aspose.cells.drawing.texts/bullet/bulletvalue/) { get; } | Bullet değerini alır. |
| [FontName](../../aspose.cells.drawing.texts/bullet/fontname/) { get; set; } | Yazı tipinin adını alır ve ayarlar. |
| [Type](../../aspose.cells.drawing.texts/bullet/type/) { get; set; } | Bullet tipini alır ve ayarlar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassBulletDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text";

            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000;

            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = 'v';
            bullet.FontName = "Arial";

            workbook.Save("TextsClassBulletDemo_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


