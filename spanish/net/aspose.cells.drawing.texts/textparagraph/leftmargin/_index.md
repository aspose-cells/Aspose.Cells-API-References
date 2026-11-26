---
title: "TextParagraph.LeftMargin"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Especifica el margen izquierdo del párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/leftmargin/
---
## TextParagraph.LeftMargin property

Especifica el margen izquierdo del párrafo.

```csharp
public double LeftMargin { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 2, 200, 200);
            textBox.Text = "This is a sample text paragraph.\nSecond line of the paragraph.";

            // Obtén el párrafo de texto del primer párrafo del cuadro de texto
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Muestre el valor actual del margen izquierdo
            Console.WriteLine("Current LeftMargin value: " + paragraph.LeftMargin);

            // Establezca un nuevo valor de margen izquierdo (en puntos)
            paragraph.LeftMargin = 20.0;

            // Demuestre el efecto agregando otro cuadro de texto con el margen predeterminado
            TextBox textBox2 = worksheet.Shapes.AddTextBox(0, 3, 2, 2, 200, 200);
            textBox2.Text = "This text box has default left margin.\nCompare the indentation.";

            // Guarde el libro de trabajo para mostrar la diferencia
            workbook.Save("TextParagraphLeftMarginDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


