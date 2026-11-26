---
title: "Bullet.BulletValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Bullet. Obtiene el valor de la viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/bullet/bulletvalue/
---
## Bullet.BulletValue property

Obtiene el valor de la viñeta.

```csharp
public BulletValue BulletValue { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class BulletPropertyBulletValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text with bullet";

            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000;

            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = 'v';
            bullet.FontName = "Arial";

            workbook.Save("BulletValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BulletValue](../../bulletvalue/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


