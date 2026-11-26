---
title: "Bullet.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Bullet. Obtiene y establece el tipo de viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/bullet/type/
---
## Bullet.Type property

Obtiene y establece el tipo de viñeta.

```csharp
public BulletType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class BulletPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text with bullet";

            // Configurar propiedades de viñetas
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character; // Demonstrating Type property usage
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Guarda el libro de trabajo
            workbook.Save("BulletPropertyTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [BulletType](../../bullettype/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


