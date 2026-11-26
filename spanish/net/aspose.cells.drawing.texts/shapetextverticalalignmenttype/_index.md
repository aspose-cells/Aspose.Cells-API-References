---
title: "Enum ShapeTextVerticalAlignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Texts.ShapeTextVerticalAlignmentType enum. Corresponde a Formato de forma  Opciones de texto  Cuadro de texto  Alineación vertical en Excel"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextverticalalignmenttype/
---
## ShapeTextVerticalAlignmentType enumeration

Corresponde a "Formato de forma - Opciones de texto - Cuadro de texto - Alineación vertical" en Excel.

```csharp
public enum ShapeTextVerticalAlignmentType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Top | `0` |  |
| Middle | `1` |  |
| Bottom | `2` |  |
| TopCentered | `3` |  |
| MiddleCentered | `4` |  |
| BottomCentered | `5` |  |
| Left | `6` |  |
| Center | `7` |  |
| Right | `8` |  |
| LeftMiddle | `9` |  |
| CenterMiddle | `10` |  |
| RightMiddle | `11` |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassShapeTextVerticalAlignmentTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar un cuadro de texto a la hoja de cálculo
                var textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 300);
                textBox.Text = "Sample text for vertical alignment demonstration";

                // Establecer alineación vertical del texto a Medio
                textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Middle;

                // Mostrar la alineación vertical actual
                Console.WriteLine("Current vertical alignment: " + textBox.TextBoxOptions.ShapeTextVerticalAlignment);

                // Cambiar a alineación superior
                textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Top;
                Console.WriteLine("Changed to: " + textBox.TextBoxOptions.ShapeTextVerticalAlignment);

                // Guarda el libro de trabajo
                workbook.Save("ShapeTextVerticalAlignmentTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapeTextVerticalAlignmentType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


