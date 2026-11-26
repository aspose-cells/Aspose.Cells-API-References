---
title: "TextParagraph.RightMargin"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Especifica el margen derecho del párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/rightmargin/
---
## TextParagraph.RightMargin property

Especifica el margen derecho del párrafo.

```csharp
public double RightMargin { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "This is a sample text to demonstrate RightMargin property of TextParagraph.";

            // Obtén el párrafo de texto del primer párrafo del cuadro de texto
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Muestre el valor actual del margen derecho
            Console.WriteLine("Current RightMargin value: " + paragraph.RightMargin);

            // Establezca un nuevo valor de margen derecho (en puntos)
            paragraph.RightMargin = 20.0;

            // Agregue otro cuadro de texto para mostrar la diferencia
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 2, 1, 2, 200, 200);
            textBox2.Text = "This text has default RightMargin for comparison.";
            
            // Guardar el libro de trabajo para ver el efecto
            workbook.Save("TextParagraphRightMarginDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


