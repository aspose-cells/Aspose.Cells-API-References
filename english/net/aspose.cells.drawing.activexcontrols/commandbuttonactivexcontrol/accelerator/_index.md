---
title: CommandButtonActiveXControl.Accelerator
second_title: Aspose.Cells for .NET API Reference
description: CommandButtonActiveXControl property. Gets and sets the accelerator key for the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/accelerator/
---
## CommandButtonActiveXControl.Accelerator property

Gets and sets the accelerator key for the control.

```csharp
public char Accelerator { get; set; }
```

### Examples

```csharp
// Called: commandButton.Accelerator = 'C';
public static void Property_Accelerator()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a CommandButton ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2,2,2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Set properties of the CommandButton ActiveX control
            commandButton.Caption = "Click Me";
            commandButton.PicturePosition = ControlPicturePositionType.Center;
            commandButton.Accelerator = 'C';
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
            commandButton.LinkedCell = "A1";
            commandButton.ListFillRange = "A2:A10";

            // Save the workbook
            workbook.Save("CommandButtonActiveXControlExample.xlsx");
            workbook.Save("CommandButtonActiveXControlExample.pdf");
        }
```

### See Also

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


