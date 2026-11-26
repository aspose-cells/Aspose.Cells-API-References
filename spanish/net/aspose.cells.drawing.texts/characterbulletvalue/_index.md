---
title: "Clase CharacterBulletValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Texts.CharacterBulletValue. Representa la viñeta de carácter"
type: docs
url: /es/net/aspose.cells.drawing.texts/characterbulletvalue/
---
## CharacterBulletValue class

Representa la viñeta de carácter.

```csharp
public class CharacterBulletValue : BulletValue
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CharacterBulletValue](characterbulletvalue/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Character](../../aspose.cells.drawing.texts/characterbulletvalue/character/) { get; set; } | Obtiene y establece el carácter de la viñeta. |
| override [Type](../../aspose.cells.drawing.texts/characterbulletvalue/type/) { get; } | Obtiene el tipo de la viñeta. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassCharacterBulletValueDemo
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

            workbook.Save("CharacterBulletValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


