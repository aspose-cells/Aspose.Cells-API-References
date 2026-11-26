---
title: "TextParagraphCollection.GetEnumerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método TextParagraphCollection. Obtiene el enumerador de los párrafos"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraphcollection/getenumerator/
---
## TextParagraphCollection.GetEnumerator method

Obtiene el enumerador de los párrafos.

```csharp
public IEnumerator GetEnumerator()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.Collections;

    public class TextParagraphCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo con todos los parámetros requeridos
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 200, 100, 100);
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Obtener la colección de párrafos de texto
            TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;

            try
            {
                // Llame al método GetEnumerator
                IEnumerator enumerator = paragraphs.GetEnumerator();

                Console.WriteLine($"Number of paragraphs: {paragraphs.Count}");
                Console.WriteLine("Paragraphs:");

                // Iterar a través de los párrafos usando el enumerador
                while (enumerator.MoveNext())
                {
                    TextParagraph paragraph = (TextParagraph)enumerator.Current;
                    Console.WriteLine(textBox.Text); // Using the text from the textbox since TextParagraph doesn't have Text property
                }

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("MethodGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


