---
title: "TextTabStopCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextTabStopCollection. Obtiene TextTabStop por el índice"
type: docs
url: /es/net/aspose.cells.drawing.texts/texttabstopcollection/item/
---
## TextTabStopCollection indexer

Obtiene [`TextTabStop`](../../texttabstop/) por el índice.

```csharp
public TextTabStop this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añadir una forma de cuadro de texto que contenga caracteres de tabulación
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 50);
            shape.Text = "Left\tCenter\tRight";

            // Acceder a la colección de paradas de tabulación del primer párrafo
            var textParagraph = shape.TextBody.TextParagraphs[0];
            var tabStops = textParagraph.Stops;

            // Preparar la colección con paradas de tabulación conocidas
            tabStops.Clear();
            tabStops.Add(TextTabAlignmentType.Left, 50);
            tabStops.Add(TextTabAlignmentType.Center, 150);
            tabStops.Add(TextTabAlignmentType.Right, 250);

            try
            {
                // Utilizar la propiedad Item (indexador) para leer una parada de tabulación específica
                TextTabStop firstStop = tabStops[0]; // Item property (read‑only)
                Console.WriteLine($"First Tab Stop -> Position: {firstStop.TabPosition}, Alignment: {firstStop.TabAlignment}");

                // Demostrar la lectura de otro elemento
                TextTabStop secondStop = tabStops[1];
                Console.WriteLine($"Second Tab Stop -> Position: {secondStop.TabPosition}, Alignment: {secondStop.TabAlignment}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error accessing Item property: {ex.Message}");
            }

            // Guardar el libro de trabajo con los cambios
            workbook.Save("TextTabStopCollectionItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextTabStop](../../texttabstop/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


