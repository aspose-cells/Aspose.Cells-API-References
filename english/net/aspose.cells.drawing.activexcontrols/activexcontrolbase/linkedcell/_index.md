---
title: ActiveXControlBase.LinkedCell
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControlBase property. Gets and sets the linked cell
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/
---
## ActiveXControlBase.LinkedCell property

Gets and sets the linked cell.

```csharp
public string LinkedCell { get; set; }
```

### Examples

```csharp
// Called: activeXControl.LinkedCell = "A1";
public static void ActiveXControlBase_Property_LinkedCell()
        {
            // Initialize a new workbook.
            Workbook workbook = new Workbook();

            // Add a SpinButtonActiveXControl.
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.SpinButton, 1, 0, 1, 0, 100, 50);
            SpinButtonActiveXControl activeXControl = (SpinButtonActiveXControl)shape.ActiveXControl;

            // Setting properties
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
            activeXControl.IsAutoSize = true;
            activeXControl.IMEMode = InputMethodEditorMode.On;
            activeXControl.TextAlign = TextAlignmentType.Center;
            activeXControl.Width = 150;
            activeXControl.Height = 30;
            activeXControl.MousePointer = ControlMousePointerType.Default;
            activeXControl.ForeOleColor = 0x000000; // Black color
            activeXControl.BackOleColor = 0xFFFFFF; // White color
            activeXControl.IsVisible = true;
            activeXControl.Shadow = false;
            activeXControl.LinkedCell = "A1";
            activeXControl.ListFillRange = "A2:A10";

            // Save the workbook
            workbook.Save("SpinButtonActiveXControlExample.xlsx");

            return;
        }
```

### See Also

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


