---
title: "Clase Bullet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Texts.Bullet. Representa los puntos de viñeta que deben aplicarse a un párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/bullet/
---
## Bullet class

Representa los puntos de viñeta que deben aplicarse a un párrafo.

```csharp
public class Bullet
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BulletValue](../../aspose.cells.drawing.texts/bullet/bulletvalue/) { get; } | Obtiene el valor de la viñeta. |
| [FontName](../../aspose.cells.drawing.texts/bullet/fontname/) { get; set; } | Obtiene y establece el nombre de la fuente. |
| [Type](../../aspose.cells.drawing.texts/bullet/type/) { get; set; } | Obtiene y establece el tipo de viñeta. |

### Ejemplos

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

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


