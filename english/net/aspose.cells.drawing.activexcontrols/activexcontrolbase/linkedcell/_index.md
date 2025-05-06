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
// Called: control.LinkedCell = &amp;quot;A1&amp;quot;;
public static void Property_LinkedCell()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);

            CheckBoxActiveXControl control = (CheckBoxActiveXControl)shape.ActiveXControl;
            control.Font.Size = 20;

            // Set properties of the ActiveX control
            control.Width = 150;
            control.Height = 30;
            control.MousePointer = ControlMousePointerType.Arrow;
            control.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            control.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Yellow);
            control.IsVisible = true;
            control.Shadow = true;
            control.LinkedCell = &quot;A1&quot;;
            control.ListFillRange = &quot;A2:A10&quot;;

            // Save the workbook
            workbook.Save(&quot;ActiveXControlBaseExample.xlsx&quot;);
            workbook.Save(&quot;ActiveXControlBaseExample.pdf&quot;, SaveFormat.Pdf);
        }
```

### See Also

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


