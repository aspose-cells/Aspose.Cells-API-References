---
title: "Enum TextTabAlignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Texts.TextTabAlignmentType enum. Representa los tipos de alineación de tabulaciones de texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/texttabalignmenttype/
---
## TextTabAlignmentType enumeration

Representa los tipos de alineación de tabulaciones de texto.

```csharp
public enum TextTabAlignmentType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Center | `0` | El texto en esta tabulación está centrado. |
| Decimal | `1` | En esta tabulación, los decimales están alineados. |
| Left | `2` | El texto en esta tabulación está alineado a la izquierda. |
| Right | `3` | El texto en esta tabulación está alineado a la derecha. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextTabAlignmentTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un cuadro de texto para demostrar alineaciones de tabulaciones
            int textBoxIndex = worksheet.TextBoxes.Add(0, 0, 400, 300);
            var textBox = worksheet.TextBoxes[textBoxIndex];
            var paragraph = textBox.TextBody.TextParagraphs[0];

            // Agrega tabulaciones con diferentes tipos de alineación
            paragraph.Stops.Add(TextTabAlignmentType.Left, 100);
            paragraph.Stops.Add(TextTabAlignmentType.Center, 200);
            paragraph.Stops.Add(TextTabAlignmentType.Right, 300);
            paragraph.Stops.Add(TextTabAlignmentType.Decimal, 400);

            // Establece texto para demostrar todos los tipos de alineación
            textBox.Text = "Left\tCenter\tRight\tDecimal\n" +
                           "Data\tData\tData\t12.34\n" +
                           "More\tMore\tMore\t56.78";

            // Aplica formato para que las tabulaciones sean visibles
            textBox.Font.Size = 12;
            textBox.TextBody.TextParagraphs[0].AlignmentType = TextAlignmentType.Left;

            // Guardar el resultado
            workbook.Save("TextTabAlignmentTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


