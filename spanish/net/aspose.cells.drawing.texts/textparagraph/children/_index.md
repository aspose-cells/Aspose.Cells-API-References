---
title: "TextParagraph.Children"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Obtiene todas las ejecuciones de texto en este párrafo. Si este párrafo está vacío, devuelve el propio párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/children/
---
## TextParagraph.Children property

Obtiene todas las ejecuciones de texto en este párrafo. Si este párrafo está vacío, devuelve el propio párrafo.

```csharp
public FontSetting[] Children { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyChildrenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 100, 200);
            textBox.Text = "First line\nSecond line\nThird line";

            // Obtener la colección de párrafos de texto
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Mostrar el número de hijos (ejecuciones de texto) en el párrafo
            Console.WriteLine("Number of children (text runs): " + textParagraph.Children.Length);

            // Modificar la configuración de fuente de cada hijo (ejecución de texto)
            foreach (FontSetting child in textParagraph.Children)
            {
                child.Font.Size = 12;
                child.Font.Color = System.Drawing.Color.Blue;
                child.Font.IsBold = true;
            }

            // Agregar otra línea con formato diferente
            textBox.Text += "\nFourth line";
            fontSetting = (FontSetting)textBox.GetCharacters()[textBox.Text.Length - 1];
            textParagraph = (TextParagraph)fontSetting;

            // Mostrar el número actualizado de hijos
            Console.WriteLine("Updated number of children: " + textParagraph.Children.Length);

            // Guarda el libro de trabajo
            workbook.Save("TextParagraphChildrenDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


