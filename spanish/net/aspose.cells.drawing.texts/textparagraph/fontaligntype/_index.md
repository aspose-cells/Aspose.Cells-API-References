---
title: "TextParagraph.FontAlignType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Determina dónde verticalmente en una línea de texto se posicionan las palabras reales. Esto trata sobre la colocación vertical de los caracteres con respecto a las líneas base"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/fontaligntype/
---
## TextParagraph.FontAlignType property

Determina dónde, verticalmente, en una línea de texto se posicionan las palabras reales. Esto trata sobre la colocación vertical de los caracteres con respecto a las líneas base.

```csharp
public TextFontAlignType FontAlignType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFontAlignTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            int textboxIndex = worksheet.TextBoxes.Add(1, 1, 200, 400);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample Text\nFor Font Alignment Demo";

            // Obtener el primer párrafo del cuadro de texto
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];

            // Mostrar el valor actual de FontAlignType
            Console.WriteLine("Current FontAlignType value: " + paragraph.FontAlignType);

            // Establecer FontAlignType a Bottom
            paragraph.FontAlignType = TextFontAlignType.Bottom;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Establecer FontAlignType a Center
            paragraph.FontAlignType = TextFontAlignType.Center;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Establecer FontAlignType a Top
            paragraph.FontAlignType = TextFontAlignType.Top;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Guardar el libro de trabajo para ver los efectos
            workbook.Save("TextParagraphPropertyFontAlignTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextFontAlignType](../../textfontaligntype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


