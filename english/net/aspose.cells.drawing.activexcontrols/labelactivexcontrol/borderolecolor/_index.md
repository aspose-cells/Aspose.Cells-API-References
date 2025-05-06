---
title: LabelActiveXControl.BorderOleColor
second_title: Aspose.Cells for .NET API Reference
description: LabelActiveXControl property. Gets and sets the ole color of the background
type: docs
url: /net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/borderolecolor/
---
## LabelActiveXControl.BorderOleColor property

Gets and sets the ole color of the background.

```csharp
public int BorderOleColor { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Label Border Color: &amp;quot; + label.BorderOleColor);
public static void Property_BorderOleColor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a Label ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Set properties for the Label
            label.Caption = &quot;Hello, Aspose!&quot;;
            label.PicturePosition = ControlPicturePositionType.Center;
            label.BorderOleColor = 0x000000; // Black color
            label.BorderStyle = ControlBorderType.Single;
            label.SpecialEffect = ControlSpecialEffectType.Flat;
            label.Accelerator = &apos;H&apos;;
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
            workbook.Save(&quot;LabelActiveXControlDemo.xlsx&quot;);

            // Output the results
            Console.WriteLine(&quot;Label Caption: &quot; + label.Caption);
            Console.WriteLine(&quot;Label Picture Position: &quot; + label.PicturePosition);
            Console.WriteLine(&quot;Label Border Color: &quot; + label.BorderOleColor);
            Console.WriteLine(&quot;Label Border Style: &quot; + label.BorderStyle);
            Console.WriteLine(&quot;Label Special Effect: &quot; + label.SpecialEffect);
            Console.WriteLine(&quot;Label Accelerator: &quot; + label.Accelerator);
            Console.WriteLine(&quot;Label Is Word Wrapped: &quot; + label.IsWordWrapped);
            Console.WriteLine(&quot;Label Is Enabled: &quot; + label.IsEnabled);
            Console.WriteLine(&quot;Label Is Locked: &quot; + label.IsLocked);
            Console.WriteLine(&quot;Label Is Transparent: &quot; + label.IsTransparent);
            Console.WriteLine(&quot;Label Is Auto Size: &quot; + label.IsAutoSize);
            Console.WriteLine(&quot;Label IME Mode: &quot; + label.IMEMode);
            Console.WriteLine(&quot;Label Text Align: &quot; + label.TextAlign);
            Console.WriteLine(&quot;Label Fore Color: &quot; + label.ForeOleColor);
            Console.WriteLine(&quot;Label Back Color: &quot; + label.BackOleColor);
            Console.WriteLine(&quot;Label Is Visible: &quot; + label.IsVisible);
            Console.WriteLine(&quot;Label Shadow: &quot; + label.Shadow);
        }
```

### See Also

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


