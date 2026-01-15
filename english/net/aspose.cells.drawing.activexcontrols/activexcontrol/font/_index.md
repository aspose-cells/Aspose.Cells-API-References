---
title: ActiveXControl.Font
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControl property. Represents the font of the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/font/
---
## ActiveXControl.Font property

Represents the font of the control.

```csharp
public Font Font { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlPropertyFontDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add an ActiveX control (Label) to the worksheet
                Shape shape = worksheet.Shapes.AddActiveXControl(
                    ControlType.Label,
                    1, 1, 200, 50,
                    0, 0);

                // Get the ActiveX control instance
                LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

                // Set some basic properties
                label.Caption = "Sample Label";

                // Access the Font property (read-only)
                Font controlFont = label.Font;

                // Display font properties
                Console.WriteLine("Font Name: " + controlFont.Name);
                Console.WriteLine("Font Size: " + controlFont.Size);
                Console.WriteLine("Is Bold: " + controlFont.IsBold);
                Console.WriteLine("Is Italic: " + controlFont.IsItalic);
                Console.WriteLine("Color: " + controlFont.Color);
                Console.WriteLine("Underline Type: " + controlFont.Underline);

                // Save the workbook
                workbook.Save("FontDemo.xlsx");
                Console.WriteLine("Font properties demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


