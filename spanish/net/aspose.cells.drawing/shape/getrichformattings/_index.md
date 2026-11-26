---
title: "Shape.GetRichFormattings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto"
type: docs
url: /es/net/aspose.cells.drawing/shape/getrichformattings/
---
## Shape.GetRichFormattings method

Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto.

```csharp
public FontSetting[] GetRichFormattings()
```

### Valor de retorno

Todos los objetos Characters

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma con texto enriquecido (recuento de parámetros correcto para AddRectangle)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is bold and this is italic";
            
            // Formatear partes del texto
            shape.Characters(0, 4).Font.IsBold = true;
            shape.Characters(13, 6).Font.IsItalic = true;

            // Obtener formatos de texto enriquecido
            FontSetting[] formattings = shape.GetRichFormattings();

            // Mostrar información de formato
            Console.WriteLine("Rich text formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"Text segment: '{shape.Text.Substring(setting.StartIndex, setting.Length)}'");
                Console.WriteLine($"Start index: {setting.StartIndex}");
                Console.WriteLine($"Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}");
                Console.WriteLine($"Italic: {setting.Font.IsItalic}");
                Console.WriteLine();
            }
        }
    }
}
```

### Ver también

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


