---
title: "TextOptions.LatinName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextOptions. Obtiene y establece el nombre latino"
type: docs
url: /es/net/aspose.cells.drawing.texts/textoptions/latinname/
---
## TextOptions.LatinName property

Obtiene y establece el nombre latino.

```csharp
public string LatinName { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyLatinNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar opciones de texto
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            shape.Text = "Sample Text";

            // Obtener las TextOptions del primer párrafo de la forma
            TextOptions textOptions = shape.TextBody.TextParagraphs[0].TextOptions;

            // Mostrar el valor actual de LatinName
            Console.WriteLine("Current LatinName value: " + textOptions.LatinName);

            // Establecer un nuevo valor de LatinName
            textOptions.LatinName = "Times New Roman";

            // Crear otra forma para comparar el renderizado de fuentes
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 3, 0, 100, 150);
            shape2.Text = "Comparison Text";
            shape2.TextBody.TextParagraphs[0].TextOptions.LatinName = "Arial";

            // Guardar el libro de trabajo para ver los efectos
            workbook.Save("PropertyLatinNameDemo.xlsx");

            // Mostrar el nuevo valor de LatinName
            Console.WriteLine("New LatinName value: " + textOptions.LatinName);
        }
    }
}
```

### Ver también

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


