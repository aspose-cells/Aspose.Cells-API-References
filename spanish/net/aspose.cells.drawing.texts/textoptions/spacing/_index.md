---
title: "TextOptions.Spacing"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextOptions. Especifica el espaciado entre caracteres dentro de una ejecución de texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/textoptions/spacing/
---
## TextOptions.Spacing property

Especifica el espaciado entre caracteres dentro de un tramo de texto.

```csharp
public double Spacing { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertySpacingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 0, 100, 200);
            textBox.Text = "Sample Text with Spacing";

            // Obtener las opciones de texto del cuadro de texto
            TextOptions textOptions = textBox.TextOptions;

            // Mostrar el valor actual del espaciado
            Console.WriteLine("Current Spacing value: " + textOptions.Spacing);

            // Establecer nuevos valores de espaciado y ver los efectos
            textOptions.Spacing = 2.0; // Increased spacing
            Console.WriteLine("Text with increased spacing (2.0)");

            // Guardar el libro con el primer espaciado
            workbook.Save("TextSpacingDemo1.xlsx");

            // Cambiar el espaciado a un valor negativo (caracteres más cercanos entre sí)
            textOptions.Spacing = -1.0;
            Console.WriteLine("Text with decreased spacing (-1.0)");

            // Guardar el libro con el segundo espaciado
            workbook.Save("TextSpacingDemo2.xlsx");

            // Restablecer al espaciado predeterminado
            textOptions.Spacing = 0.0;
            Console.WriteLine("Text with default spacing (0.0)");

            // Guardar el libro con el espaciado predeterminado
            workbook.Save("TextSpacingDemo3.xlsx");
        }
    }
}
```

### Ver también

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


