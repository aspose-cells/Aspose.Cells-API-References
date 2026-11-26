---
title: "Shape.TextBoxOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Obtiene la información de texto en el shape"
type: docs
url: /es/net/aspose.cells.drawing/shape/textboxoptions/
---
## Shape.TextBoxOptions property

Obtiene la información de texto en la forma

```csharp
public TextBoxOptions TextBoxOptions { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;

    public class ShapePropertyTextBoxOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto
            int textBoxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "This is a sample text box to demonstrate TextBoxOptions properties.";

            // Mostrar las propiedades actuales de TextBoxOptions
            TextBoxOptions textBoxOptions = textBox.TextBoxOptions;
            Console.WriteLine("Current TextBoxOptions:");
            Console.WriteLine("Vertical Alignment: " + textBoxOptions.ShapeTextVerticalAlignment);
            Console.WriteLine("Resize To Fit Text: " + textBoxOptions.ResizeToFitText);
            Console.WriteLine("Text Direction: " + textBoxOptions.ShapeTextDirection);
            Console.WriteLine("Left Margin: " + textBoxOptions.LeftMarginPt + " pt");
            Console.WriteLine("Right Margin: " + textBoxOptions.RightMarginPt + " pt");

            // Modificar las propiedades de TextBoxOptions
            textBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Middle;
            textBoxOptions.ResizeToFitText = true;
            textBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;
            textBoxOptions.LeftMarginPt = 10;
            textBoxOptions.RightMarginPt = 10;
            textBoxOptions.TopMarginPt = 5;
            textBoxOptions.BottomMarginPt = 5;

            // Guarda el libro de trabajo
            workbook.Save("TextBoxOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxOptions](../../../aspose.cells.drawing.texts/textboxoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


