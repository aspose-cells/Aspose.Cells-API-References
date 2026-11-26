---
title: "TextParagraph.Stops"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Obtiene la lista de tabulaciones"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/stops/
---
## TextParagraph.Stops property

Obtiene la lista de tabulaciones.

```csharp
public TextTabStopCollection Stops { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyStopsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar texto a una celda y obtener sus propiedades de párrafo de texto
            worksheet.Cells["A1"].PutValue("Sample\tText\tWith\tTabs");
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            shape.Text = "Sample\tText\tWith\tTabs";
            
            // Obtener el párrafo de texto
            var textOptions = shape.TextBody.TextParagraphs[0];

            // Mostrar el recuento actual de tabulaciones
            Console.WriteLine("Current tab stops count: " + textOptions.Stops.Count);

            // Agregar nuevas tabulaciones
            textOptions.Stops.Add(TextTabAlignmentType.Left, 50);
            textOptions.Stops.Add(TextTabAlignmentType.Center, 100);
            textOptions.Stops.Add(TextTabAlignmentType.Right, 150);

            // Mostrar tabulaciones actualizadas
            Console.WriteLine("Updated tab stops count: " + textOptions.Stops.Count);
            for (int i = 0; i < textOptions.Stops.Count; i++)
            {
                Console.WriteLine($"Tab {i+1}: Position={textOptions.Stops[i].TabPosition}, Alignment={textOptions.Stops[i].TabAlignment}");
            }

            // Guardar el libro de trabajo para ver el efecto
            workbook.Save("TextParagraphStopsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextTabStopCollection](../../texttabstopcollection/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


