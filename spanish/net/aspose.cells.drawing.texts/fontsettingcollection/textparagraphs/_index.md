---
title: "FontSettingCollection.TextParagraphs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontSettingCollection. Obtiene todos los párrafos"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/
---
## FontSettingCollection.TextParagraphs property

Obtiene todos los párrafos.

```csharp
public TextParagraphCollection TextParagraphs { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un cuadro de texto a la hoja de cálculo
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "First paragraph\nSecond paragraph";

            // Accede al primer párrafo de texto
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            
            // Establece las propiedades de interlineado
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000; // 300% line spacing

            // Establece las propiedades de viñetas
            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Guarda el libro de trabajo
            workbook.Save("TextParagraphsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextParagraphCollection](../../textparagraphcollection/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


