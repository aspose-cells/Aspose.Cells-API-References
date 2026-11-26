---
title: "TextParagraph.FirstLineIndent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Especifica el tamaño de sangría que se aplicará a la primera línea de texto del párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/firstlineindent/
---
## TextParagraph.FirstLineIndent property

Especifica el tamaño de sangría que se aplicará a la primera línea de texto del párrafo.

```csharp
public double FirstLineIndent { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFirstLineIndentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 100, 300, 200, 100);
            textBox.Text = "This is a sample paragraph with multiple lines.\nFirst line should have indent.\nSecond line should be normal.";

            // Obtenga el párrafo de texto del cuadro de texto
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Muestre el valor actual de FirstLineIndent
            Console.WriteLine("Current FirstLineIndent value: " + textParagraph.FirstLineIndent);

            // Establezca un nuevo valor de FirstLineIndent (20 puntos)
            textParagraph.FirstLineIndent = 20;
            Console.WriteLine("FirstLineIndent set to: " + textParagraph.FirstLineIndent);

            // Agregue otro cuadro de texto para comparar con la sangría predeterminada
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 5, 150, 300, 200, 100);
            textBox2.Text = "This is a comparison paragraph without indent.\nFirst line has no indent.\nSecond line is normal.";

            // Guardar el libro de trabajo para ver los efectos
            workbook.Save("TextParagraphPropertyFirstLineIndentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


