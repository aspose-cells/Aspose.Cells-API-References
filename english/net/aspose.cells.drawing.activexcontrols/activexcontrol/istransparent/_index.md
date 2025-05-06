---
title: ActiveXControl.IsTransparent
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControl property. Indicates whether the control is transparent
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/
---
## ActiveXControl.IsTransparent property

Indicates whether the control is transparent.

```csharp
public bool IsTransparent { get; set; }
```

### Examples

```csharp
// Called: textBoxControl.IsTransparent = false;
public static void Property_IsTransparent()
        {
            // Initialize a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a TextBox ActiveX control to the worksheet
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Set the IME mode to Full-width Hiragana
            textBoxControl.IMEMode = InputMethodEditorMode.Hiragana;

            // Set other properties for demonstration
            textBoxControl.Text = &quot;This is a test.&quot;;
            textBoxControl.IsEnabled = true;
            textBoxControl.IsLocked = false;
            textBoxControl.IsTransparent = false;
            textBoxControl.IsAutoSize = true;
            textBoxControl.Width = 200;
            textBoxControl.Height = 50;
            textBoxControl.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);
            textBoxControl.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.White);
            textBoxControl.IsVisible = true;
            textBoxControl.Shadow = false;

            // Save the workbook
            workbook.Save(&quot;InputMethodEditorModeExample.xlsx&quot;);
            workbook.Save(&quot;InputMethodEditorModeExample.pdf&quot;);
            return;
        }
```

### See Also

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


