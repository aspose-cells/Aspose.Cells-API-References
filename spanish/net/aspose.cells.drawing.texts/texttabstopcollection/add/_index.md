---
title: "TextTabStopCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método TextTabStopCollection. Añade una parada de tabulación"
type: docs
url: /es/net/aspose.cells.drawing.texts/texttabstopcollection/add/
---
## TextTabStopCollection.Add method

Agrega una tabulación.

```csharp
public int Add(TextTabAlignmentType tabAlignment, double tabPosition)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tabAlignment | TextTabAlignmentType |  |
| tabPosition | Double |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopCollectionMethodAddWithTextTabAlignmentTypeDoubleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para añadir texto con paradas de tabulación
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            var textParagraph = shape.TextBody.TextParagraphs[0];
            
            // Obtener el TextTabStopCollection
            var tabStops = textParagraph.Stops;

            try
            {
                // Llamar al método Add con TextTabAlignmentType.Left y posición 50.0
                int index1 = tabStops.Add(TextTabAlignmentType.Left, 50.0);
                
                // Llamar al método Add con TextTabAlignmentType.Right y posición 100.0
                int index2 = tabStops.Add(TextTabAlignmentType.Right, 100.0);
                
                // Añadir texto con tabulaciones para demostrar las paradas de tabulación
                shape.Text = "Left-aligned\tRight-aligned";

                Console.WriteLine("Added tab stops at positions 50.0 (Left) and 100.0 (Right)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("TextTabStopCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextTabAlignmentType](../../texttabalignmenttype/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


