---
title: "Enum TextFontAlignType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Drawing.Texts.TextFontAlignType. Representa los diferentes tipos de alineación de fuente"
type: docs
url: /es/net/aspose.cells.drawing.texts/textfontaligntype/
---
## TextFontAlignType enumeration

Representa los diferentes tipos de alineación de fuente.

```csharp
public enum TextFontAlignType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` | Cuando el flujo de texto es horizontal o vertical simple es igual a fontBaseline, pero para otros modos verticales es igual a fontCenter. |
| Bottom | `1` | Las letras están ancladas al extremo inferior de una sola línea. |
| Baseline | `2` | Las letras están ancladas a la línea base inferior de una sola línea. |
| Center | `3` | Las letras están ancladas entre las dos líneas base de una sola línea. |
| Top | `4` | Las letras están ancladas a la línea base superior de una sola línea. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextFontAlignTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear cuadros de texto con diferentes alineaciones de fuente
            var textBoxAuto = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            textBoxAuto.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Automatic;
            textBoxAuto.Text = "Automatic Alignment";

            var textBoxBottom = worksheet.Shapes.AddTextBox(0, 200, 100, 100, 200, 200);
            textBoxBottom.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Bottom;
            textBoxBottom.Text = "Bottom Alignment";

            var textBoxBaseline = worksheet.Shapes.AddTextBox(0, 400, 100, 100, 200, 200);
            textBoxBaseline.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Baseline;
            textBoxBaseline.Text = "Baseline Alignment";

            var textBoxCenter = worksheet.Shapes.AddTextBox(200, 0, 100, 100, 200, 200);
            textBoxCenter.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Center;
            textBoxCenter.Text = "Center Alignment";

            var textBoxTop = worksheet.Shapes.AddTextBox(200, 200, 100, 100, 200, 200);
            textBoxTop.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Top;
            textBoxTop.Text = "Top Alignment";

            // Mostrar todos los valores de enumeración en la consola
            Console.WriteLine("TextFontAlignType values:");
            Console.WriteLine($"Automatic: {TextFontAlignType.Automatic}");
            Console.WriteLine($"Bottom: {TextFontAlignType.Bottom}");
            Console.WriteLine($"Baseline: {TextFontAlignType.Baseline}");
            Console.WriteLine($"Center: {TextFontAlignType.Center}");
            Console.WriteLine($"Top: {TextFontAlignType.Top}");

            // Guarda el libro de trabajo
            workbook.Save("TextFontAlignTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


