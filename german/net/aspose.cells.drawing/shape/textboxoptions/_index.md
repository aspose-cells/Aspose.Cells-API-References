---
title: "Shape.TextBoxOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Liefert die Textinformationen im shape"
type: docs
url: /de/net/aspose.cells.drawing/shape/textboxoptions/
---
## Shape.TextBoxOptions property

Liest die Textinformationen in der Form.

```csharp
public TextBoxOptions TextBoxOptions { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Textfeldform hinzu
            int textBoxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "This is a sample text box to demonstrate TextBoxOptions properties.";

            // Zeige aktuelle TextBoxOptions-Eigenschaften an
            TextBoxOptions textBoxOptions = textBox.TextBoxOptions;
            Console.WriteLine("Current TextBoxOptions:");
            Console.WriteLine("Vertical Alignment: " + textBoxOptions.ShapeTextVerticalAlignment);
            Console.WriteLine("Resize To Fit Text: " + textBoxOptions.ResizeToFitText);
            Console.WriteLine("Text Direction: " + textBoxOptions.ShapeTextDirection);
            Console.WriteLine("Left Margin: " + textBoxOptions.LeftMarginPt + " pt");
            Console.WriteLine("Right Margin: " + textBoxOptions.RightMarginPt + " pt");

            // Ändere TextBoxOptions-Eigenschaften
            textBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Middle;
            textBoxOptions.ResizeToFitText = true;
            textBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;
            textBoxOptions.LeftMarginPt = 10;
            textBoxOptions.RightMarginPt = 10;
            textBoxOptions.TopMarginPt = 5;
            textBoxOptions.BottomMarginPt = 5;

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxOptionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxOptions](../../../aspose.cells.drawing.texts/textboxoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


