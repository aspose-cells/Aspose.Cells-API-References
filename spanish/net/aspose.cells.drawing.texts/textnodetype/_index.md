---
title: "Enumeración TextNodeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.Texts.TextNodeType. Representa el tipo de nodo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textnodetype/
---
## TextNodeType enumeration

Representa el tipo de nodo.

```csharp
public enum TextNodeType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| TextRun | `0` | Representa el nodo de texto. |
| TextParagraph | `1` | Representa el párrafo de texto. |
| Equation | `2` | Representa el texto de la ecuación. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextNodeTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un cuadro de texto y obtén sus párrafos de texto
            int textboxIndex = worksheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.TextBody.AppendText("Sample text with ");
            textbox.TextBody.AppendText("different node types");
            
            // Demuestra el uso de TextNodeType
            foreach (TextParagraph paragraph in textbox.TextBody.TextParagraphs)
            {
                foreach (FontSetting portion in paragraph.Children)
                {
                    // Obtén la porción de texto usando StartIndex y Length
                    string portionText = textbox.Text.Substring(portion.StartIndex, portion.Length);
                    Console.WriteLine("Text: " + portionText);
                    Console.WriteLine("Node Type: " + portion.Type.ToString());
                    
                    // Ejemplo de verificación del tipo de nodo
                    if (portion.Type == TextNodeType.TextRun)
                    {
                        portion.Font.Color = System.Drawing.Color.Red;
                    }
                    else if (portion.Type == TextNodeType.Equation)
                    {
                        portion.Font.Color = System.Drawing.Color.Blue;
                    }
                }
            }

            // Guardar el resultado
            workbook.Save("TextNodeTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


