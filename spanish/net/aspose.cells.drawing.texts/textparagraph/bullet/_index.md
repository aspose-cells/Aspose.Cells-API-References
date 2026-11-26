---
title: "TextParagraph.Bullet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Obtiene la viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/bullet/
---
## TextParagraph.Bullet property

Obtiene la viñeta.

```csharp
public Bullet Bullet { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyBulletDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Establecer texto y configurar el párrafo
            textbox.Text = "First Item\nSecond Item";
            textbox.TextBody.TextParagraphs[0].LineSpaceSizeType = LineSpaceSizeType.Percentage;
            textbox.TextBody.TextParagraphs[0].LineSpace = 3000;

            // Configurar viñeta para el primer párrafo
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Guarda el libro de trabajo
            workbook.Save("TextParagraphPropertyBulletDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Bullet](../../bullet/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


