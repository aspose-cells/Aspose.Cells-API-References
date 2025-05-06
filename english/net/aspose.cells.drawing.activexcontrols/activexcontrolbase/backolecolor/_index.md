---
title: ActiveXControlBase.BackOleColor
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControlBase property. Gets and sets the ole color of the background
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/
---
## ActiveXControlBase.BackOleColor property

Gets and sets the ole color of the background.

```csharp
public virtual int BackOleColor { get; set; }
```

### Examples

```csharp
// Called: controlBase.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
public static void Property_BackOleColor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl control = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Cast the ActiveXControl to ActiveXControlBase to access its properties
            ActiveXControlBase controlBase = control as ActiveXControlBase;

            if (controlBase != null)
            {
                // Set the mouse pointer type for the control
                controlBase.MousePointer = ControlMousePointerType.Cross;

                // Set other properties for demonstration
                controlBase.Width = 150;
                controlBase.Height = 50;
                controlBase.IsVisible = true;
                controlBase.Shadow = true;
                controlBase.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
                controlBase.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            }

            // Save the workbook
            workbook.Save(&quot;ControlMousePointerTypeExample.xlsx&quot;);
            workbook.Save(&quot;ControlMousePointerTypeExample.pdf&quot;);

            // Output the result
            Console.WriteLine(&quot;Workbook with ActiveX control and custom mouse pointer type saved as &apos;ControlMousePointerTypeExample.xlsx&apos;.&quot;);
        }
```

### See Also

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


