---
title: ListBoxActiveXControl.ScrollBars
second_title: Aspose.Cells for .NET API Reference
description: ListBoxActiveXControl property. Indicates specifies whether the control has vertical scroll bars horizontal scroll bars both or neither
type: docs
url: /net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/scrollbars/
---
## ListBoxActiveXControl.ScrollBars property

Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Examples

```csharp
// Called: listBoxControl.ScrollBars = ControlScrollBarType.BarsBoth;
public static void Property_ScrollBars()
        {
            // Initialize a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a ListBox ActiveX control to the worksheet
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            ListBoxActiveXControl listBoxControl = (ListBoxActiveXControl)shape.ActiveXControl;

            // Set the ScrollBars property to display both horizontal and vertical scroll bars
            listBoxControl.ScrollBars = ControlScrollBarType.BarsBoth;

            // Save the workbook
            workbook.Save("ControlScrollBarTypeExample.xlsx");
            workbook.Save("ControlScrollBarTypeExample.pdf");
            return;
        }
```

### See Also

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


