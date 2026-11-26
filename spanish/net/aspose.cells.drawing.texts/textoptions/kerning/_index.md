---
title: "TextOptions.Kerning"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextOptions. Especifica el tamaño mínimo de fuente en el que se producirá el interletraje de caracteres para este fragmento de texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/textoptions/kerning/
---
## TextOptions.Kerning property

Especifica el tamaño mínimo de fuente en el que se aplicará el interletraje de caracteres para este tramo de texto.

```csharp
public double Kerning { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyKerningDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma con texto para demostrar el interletraje
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Kerning Demonstration Text";

            // Obtener las TextOptions de la forma
            TextOptions textOptions = shape.TextOptions;

            // Mostrar el valor actual del interletraje
            Console.WriteLine("Current Kerning value: " + textOptions.Kerning);

            // Establecer interletraje a 12 puntos (tamaño de fuente mínimo para que se aplique el interletraje)
            textOptions.Kerning = 12;

            // Establecer un tamaño de fuente mayor para observar el efecto del interletraje
            textOptions.Size = 24;

            // Guardar el libro de trabajo para ver el efecto
            workbook.Save("PropertyKerningDemo.xlsx");

            // Crear otra forma con un interletraje diferente para comparar
            var shape2 = worksheet.Shapes.AddTextBox(10, 0, 1, 0, 200, 100);
            shape2.Text = "Comparison Text Without Kerning";
            shape2.TextOptions.Size = 24;
            shape2.TextOptions.Kerning = 0; // No kerning

            // Guardar de nuevo con ambos ejemplos
            workbook.Save("PropertyKerningDemoWithComparison.xlsx");
        }
    }
}
```

### Ver también

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


