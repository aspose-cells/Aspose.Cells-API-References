---
title: "TextOptions.UnderlineColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextOptions. Obtiene o establece el color del subrayado"
type: docs
url: /es/net/aspose.cells.drawing.texts/textoptions/underlinecolor/
---
## TextOptions.UnderlineColor property

Obtiene o establece el color del subrayado.

```csharp
public CellsColor UnderlineColor { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyUnderlineColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma con texto para demostrar las opciones de texto
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Underline Color Demo";
            
            // Obtener el TextOptions de la forma
            TextOptions textOptions = shape.TextOptions;

            try
            {
                // Mostrar el valor actual de UnderlineColor
                CellsColor currentColor = textOptions.UnderlineColor;
                Console.WriteLine($"Current UnderlineColor - Type: {currentColor.Type}, Color: {currentColor.Color}");

                // Establecer un nuevo UnderlineColor (ya que la propiedad es de lectura y escritura)
                CellsColor newColor = textOptions.UnderlineColor; // Use existing color object
                newColor.Color = System.Drawing.Color.Red;
                textOptions.UnderlineColor = newColor;

                // Habilitar el subrayado para ver el efecto
                textOptions.Underline = FontUnderlineType.Single;

                // Mostrar el nuevo valor de UnderlineColor
                Console.WriteLine($"New UnderlineColor - Type: {textOptions.UnderlineColor.Type}, Color: {textOptions.UnderlineColor.Color}");

                // Guardar el libro de trabajo para ver el efecto
                workbook.Save("UnderlineColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


