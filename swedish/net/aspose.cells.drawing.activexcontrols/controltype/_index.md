---
title: "Enum ControlType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlType enum. Representerar alla typer av ActiveX-kontroller"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/controltype/
---
## ControlType enumeration

Representerar alla typer av ActiveX-kontroll.

```csharp
public enum ControlType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| CommandButton | `0` | Knapp |
| ComboBox | `1` | Kombinationsruta |
| CheckBox | `2` | Kryssruta |
| ListBox | `3` | Listruta |
| TextBox | `4` | Textruta |
| SpinButton | `5` | Snurrkontroll |
| RadioButton | `6` | Radioknapp |
| Label | `7` | Etikett |
| Image | `8` | Bild |
| ToggleButton | `9` | ToggleButton |
| ScrollBar | `10` | Rullningslist |
| BarCode | `11` | Rullningslist |
| Unknown | `12` | Okänd |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlTypeDemo
    {
        public static void ControlTypeExample()
        {
            // Initiera en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en CommandButton ActiveX-kontroll
            Shape commandButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 1, 0, 1, 0, 100, 30);
            ActiveXControl commandButtonControl = commandButtonShape.ActiveXControl;
            commandButtonControl.IsEnabled = true;
            commandButtonControl.IsVisible = true;

            // Lägg till en ComboBox ActiveX-kontroll
            Shape comboBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 1, 0, 100, 30);
            ActiveXControl comboBoxControl = comboBoxShape.ActiveXControl;
            comboBoxControl.IsEnabled = true;
            comboBoxControl.IsVisible = true;

            // Lägg till en CheckBox ActiveX-kontroll
            Shape checkBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 0, 100, 30);
            ActiveXControl checkBoxControl = checkBoxShape.ActiveXControl;
            checkBoxControl.IsEnabled = true;
            checkBoxControl.IsVisible = true;

            // Lägg till en ListBox ActiveX-kontroll
            Shape listBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 7, 0, 1, 0, 100, 30);
            ActiveXControl listBoxControl = listBoxShape.ActiveXControl;
            listBoxControl.IsEnabled = true;
            listBoxControl.IsVisible = true;

            // Lägg till en TextBox ActiveX-kontroll
            Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 9, 0, 1, 0, 100, 30);
            ActiveXControl textBoxControl = textBoxShape.ActiveXControl;
            textBoxControl.IsEnabled = true;
            textBoxControl.IsVisible = true;

            // Lägg till en SpinButton ActiveX-kontroll
            Shape spinButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 11, 0, 1, 0, 100, 30);
            ActiveXControl spinButtonControl = spinButtonShape.ActiveXControl;
            spinButtonControl.IsEnabled = true;
            spinButtonControl.IsVisible = true;

            // Lägg till en RadioButton ActiveX-kontroll
            Shape radioButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 13, 0, 1, 0, 100, 30);
            ActiveXControl radioButtonControl = radioButtonShape.ActiveXControl;
            radioButtonControl.IsEnabled = true;
            radioButtonControl.IsVisible = true;

            // Lägg till en Label ActiveX-kontroll
            Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 15, 0, 1, 0, 100, 30);
            ActiveXControl labelControl = labelShape.ActiveXControl;
            labelControl.IsEnabled = true;
            labelControl.IsVisible = true;

            // Lägg till en Image ActiveX-kontroll
            Shape imageShape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 17, 0, 1, 0, 100, 30);
            ActiveXControl imageControl = imageShape.ActiveXControl;
            imageControl.IsEnabled = true;
            imageControl.IsVisible = true;

            // Lägg till en ToggleButton ActiveX-kontroll
            Shape toggleButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 19, 0, 1, 0, 100, 30);
            ActiveXControl toggleButtonControl = toggleButtonShape.ActiveXControl;
            toggleButtonControl.IsEnabled = true;
            toggleButtonControl.IsVisible = true;

            // Lägg till en ScrollBar ActiveX-kontroll
            Shape scrollBarShape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 21, 0, 1, 0, 100, 30);
            ActiveXControl scrollBarControl = scrollBarShape.ActiveXControl;
            scrollBarControl.IsEnabled = true;
            scrollBarControl.IsVisible = true;
                       

            // Spara arbetsboken
            workbook.Save("ControlTypeExample.xlsx");
            workbook.Save("ControlTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


