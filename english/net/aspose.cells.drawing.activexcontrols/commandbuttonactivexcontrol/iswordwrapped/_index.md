---
title: CommandButtonActiveXControl.IsWordWrapped
second_title: Aspose.Cells for .NET API Reference
description: CommandButtonActiveXControl property. Indicates whether the contents of the control automatically wrap at the end of a line
type: docs
url: /net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/iswordwrapped/
---
## CommandButtonActiveXControl.IsWordWrapped property

Indicates whether the contents of the control automatically wrap at the end of a line.

```csharp
public bool IsWordWrapped { get; set; }
```

### Examples

```csharp
// Called: commandButton.IsWordWrapped = true;
public static void Property_IsWordWrapped()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a CommandButton ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2,2,2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Set properties of the CommandButton ActiveX control
            commandButton.Caption = &quot;Click Me&quot;;
            commandButton.PicturePosition = ControlPicturePositionType.Center;
            commandButton.Accelerator = &apos;C&apos;;
            commandButton.TakeFocusOnClick = true;
            commandButton.IsWordWrapped = true;
            commandButton.IsEnabled = true;
            commandButton.IsLocked = false;
            commandButton.IsTransparent = false;
            commandButton.IsAutoSize = false;
            commandButton.IMEMode = InputMethodEditorMode.NoControl;
            commandButton.TextAlign = TextAlignmentType.Center;
            commandButton.Width = 150;
            commandButton.Height = 50;
            commandButton.MousePointer = ControlMousePointerType.Default;
            commandButton.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
            commandButton.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            commandButton.IsVisible = true;
            commandButton.Shadow = true;
            commandButton.LinkedCell = &quot;A1&quot;;
            commandButton.ListFillRange = &quot;A2:A10&quot;;

            // Save the workbook
            workbook.Save(&quot;CommandButtonActiveXControlExample.xlsx&quot;);
            workbook.Save(&quot;CommandButtonActiveXControlExample.pdf&quot;);
        }
```

### See Also

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


