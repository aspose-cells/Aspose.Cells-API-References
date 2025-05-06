---
title: ActiveXControl.IsEnabled
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControl property. Indicates whether the control can receive the focus and respond to usergenerated events
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/
---
## ActiveXControl.IsEnabled property

Indicates whether the control can receive the focus and respond to user-generated events.

```csharp
public bool IsEnabled { get; set; }
```

### Examples

```csharp
// Called: activeXControl.IsEnabled = true;
public static void Property_IsEnabled()
        {
            // Initialize a new workbook.
            Workbook workbook = new Workbook();

            // Add a ScrollBarActiveXControl.
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 50);
            ScrollBarActiveXControl activeXControl = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Setting properties
            activeXControl.LargeChange = 5;
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            activeXControl.IsEnabled = true;
            activeXControl.IsLocked = false;
            activeXControl.IsTransparent = false;
            activeXControl.IsAutoSize = false;
            activeXControl.IMEMode = InputMethodEditorMode.NoControl;
            activeXControl.TextAlign = TextAlignmentType.Center;
            activeXControl.Width = 100;
            activeXControl.Height = 50;
            activeXControl.MousePointer = ControlMousePointerType.Default;
            activeXControl.ForeOleColor = 0x000000; // Black color
            activeXControl.BackOleColor = 0xFFFFFF; // White color
            activeXControl.IsVisible = true;
            activeXControl.Shadow = false;
            activeXControl.LinkedCell = &quot;A1&quot;;
            activeXControl.ListFillRange = &quot;A2:A10&quot;;

            // Save the Excel file.
            workbook.Save(&quot;ScrollBarActiveXControlExample.xlsx&quot;);
        }
```

### See Also

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


