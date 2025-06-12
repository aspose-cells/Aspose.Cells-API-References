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
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyFontDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create a scroll bar shape which will create the ActiveX control
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 1, 100, 30, 100, 30);
            
            // Get the ActiveX control properties
            var control = scrollBar.ActiveXControl as Aspose.Cells.Drawing.ActiveXControls.ScrollBarActiveXControl;
            
            // Set control properties
            control.LargeChange = 1;
            control.Min = 0;
            control.Max = 32767;
            control.Position = 0;
            control.SmallChange = 1;
            
            // Set font properties through the Shape's Font property
            scrollBar.Font.Name = "MS Sans Serif";
            scrollBar.Font.Size = 8;
            
            // Save the workbook
            workbook.Save("ActiveXControlFontDemo.xlsx");
            
            Console.WriteLine("ActiveX control with font property set successfully.");
        }
    }
}
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


