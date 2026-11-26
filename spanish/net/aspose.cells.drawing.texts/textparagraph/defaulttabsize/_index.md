---
title: "TextParagraph.DefaultTabSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de TextParagraph. Obtiene y establece el tamaño predeterminado para un carácter de tabulación dentro de este párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/defaulttabsize/
---
## TextParagraph.DefaultTabSize property

Obtiene y establece el tamaño predeterminado para un carácter de tabulación dentro de este párrafo.

```csharp
public double DefaultTabSize { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyDefaultTabSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 200);
            textBox.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Obtén el párrafo de texto del primer párrafo del cuadro de texto
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Muestra el tamaño de tabulación predeterminado actual
            Console.WriteLine("Current DefaultTabSize: " + paragraph.DefaultTabSize);

            // Establezca un tamaño de tabulación más pequeño (el valor predeterminado suele ser alrededor de 36 puntos)
            paragraph.DefaultTabSize = 20.0;
            Console.WriteLine("DefaultTabSize set to: " + paragraph.DefaultTabSize);

            // Agregue otro cuadro de texto con el tamaño de tabulación predeterminado para comparar
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 3, 1, 3, 300, 200);
            textBox2.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Guarde el libro de trabajo para ver la diferencia en el espaciado de tabulaciones
            workbook.Save("TextParagraphDefaultTabSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


