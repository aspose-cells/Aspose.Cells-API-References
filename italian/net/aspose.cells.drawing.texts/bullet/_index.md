---
title: "Classe Bullet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Texts.Bullet. Rappresenta i punti elenco da applicare a un paragrafo"
type: docs
url: /it/net/aspose.cells.drawing.texts/bullet/
---
## Bullet class

Rappresenta i punti elenco che devono essere applicati a un paragrafo.

```csharp
public class Bullet
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BulletValue](../../aspose.cells.drawing.texts/bullet/bulletvalue/) { get; } | Ottiene il valore del bullet. |
| [FontName](../../aspose.cells.drawing.texts/bullet/fontname/) { get; set; } | Ottiene e imposta il nome del font. |
| [Type](../../aspose.cells.drawing.texts/bullet/type/) { get; set; } | Ottiene e imposta il tipo di bullet. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


