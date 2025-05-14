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
// Called: label.BackOleColor = 0xFFFFFF; // White color
public static void ActiveXControlBase_Property_BackOleColor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a Label ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Set properties for the Label
            label.Caption = "Hello, Aspose!";
            label.PicturePosition = ControlPicturePositionType.Center;
            label.BorderOleColor = 0x000000; // Black color
            label.BorderStyle = ControlBorderType.Single;
            label.SpecialEffect = ControlSpecialEffectType.Flat;
            label.Accelerator = 'H';
            label.IsWordWrapped = true;
            label.IsEnabled = true;
            label.IsLocked = false;
            label.IsTransparent = false;
            label.IsAutoSize = true;
            label.IMEMode = InputMethodEditorMode.NoControl;
            label.TextAlign = TextAlignmentType.Center;
            label.ForeOleColor = 0x000000; // Black color
            label.BackOleColor = 0xFFFFFF; // White color
            label.IsVisible = true;
            label.Shadow = false;

            // Save the workbook
            workbook.Save("LabelActiveXControlDemo.xlsx");

            // Output the results
            Console.WriteLine("Label Caption: " + label.Caption);
            Console.WriteLine("Label Picture Position: " + label.PicturePosition);
            Console.WriteLine("Label Border Color: " + label.BorderOleColor);
            Console.WriteLine("Label Border Style: " + label.BorderStyle);
            Console.WriteLine("Label Special Effect: " + label.SpecialEffect);
            Console.WriteLine("Label Accelerator: " + label.Accelerator);
            Console.WriteLine("Label Is Word Wrapped: " + label.IsWordWrapped);
            Console.WriteLine("Label Is Enabled: " + label.IsEnabled);
            Console.WriteLine("Label Is Locked: " + label.IsLocked);
            Console.WriteLine("Label Is Transparent: " + label.IsTransparent);
            Console.WriteLine("Label Is Auto Size: " + label.IsAutoSize);
            Console.WriteLine("Label IME Mode: " + label.IMEMode);
            Console.WriteLine("Label Text Align: " + label.TextAlign);
            Console.WriteLine("Label Fore Color: " + label.ForeOleColor);
            Console.WriteLine("Label Back Color: " + label.BackOleColor);
            Console.WriteLine("Label Is Visible: " + label.IsVisible);
            Console.WriteLine("Label Shadow: " + label.Shadow);
        }
```

### See Also

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


