---
title: "Enum BulletType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Texts.BulletType enum. Representa el tipo de viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/bullettype/
---
## BulletType enumeration

Representa el tipo de viñeta.

```csharp
public enum BulletType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin viñeta. |
| Character | `1` | Viñeta de carácter. |
| Picture | `2` | Viñeta de imagen. |
| AutoNumbered | `3` | Viñeta numerada automática. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassBulletTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un TextBox y establece texto
            TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "Sample text with bullet type demonstration";

            // Crear opciones de viñetas
            NoneBulletValue noneBullet = new NoneBulletValue();
            BulletType bulletType = noneBullet.Type;

            // Aplicar configuraciones de viñetas a los párrafos de texto
            foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
            {
                paragraph.Bullet.Type = bulletType;
            }

            Console.WriteLine("Bullet Type applied: " + bulletType);
            workbook.Save("BulletTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


