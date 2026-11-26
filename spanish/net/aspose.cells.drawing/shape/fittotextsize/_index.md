---
title: "Shape.FitToTextSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Recalcular un área de texto adecuada para mostrar todo el contenido del texto"
type: docs
url: /es/net/aspose.cells.drawing/shape/fittotextsize/
---
## Shape.FitToTextSize method

Recalcula un área de texto adecuada para mostrar todo el contenido de texto.

```csharp
public void FitToTextSize()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeMethodFitToTextSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 100);
            textBox.Text = "This is a sample text that will demonstrate the FitToTextSize method functionality.";

            try
            {
                // Mostrar dimensiones originales
                Console.WriteLine($"Original Width: {textBox.Width}, Height: {textBox.Height}");

                // Llamar al método FitToTextSize
                textBox.FitToTextSize();

                // Mostrar dimensiones ajustadas
                Console.WriteLine($"Adjusted Width: {textBox.Width}, Height: {textBox.Height}");
                Console.WriteLine("FitToTextSize method executed successfully");

                // Agregar más texto para mostrar el efecto
                textBox.Text += " Adding more text to show how the shape adjusts to fit the content.";
                textBox.FitToTextSize();
                Console.WriteLine($"Final Width: {textBox.Width}, Height: {textBox.Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FitToTextSize method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("ShapeMethodFitToTextSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


