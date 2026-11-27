---
title: "Enum ControlSpecialEffectType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlSpecialEffectType enum. Representerar typen av specialeffekt"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/controlspecialeffecttype/
---
## ControlSpecialEffectType enumeration

Representerar typen av specialeffekt.

```csharp
public enum ControlSpecialEffectType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Flat | `0` | Platt |
| Raised | `1` | Upphöjd |
| Sunken | `2` | Nedsänkt |
| Etched | `3` | Graverad |
| Bump | `6` | Bula |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlSpecialEffectTypeDemo
    {
        public static void ControlSpecialEffectTypeExample()
        {
            // Initiera en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en CheckBox ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
            CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper för CheckBox ActiveX-kontrollen
            checkBoxControl.Caption = "Example CheckBox";
            checkBoxControl.SpecialEffect = ControlSpecialEffectType.Raised;

            // Lägg till en ComboBox ActiveX-kontroll
            shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 3, 0, 100, 50);
            ComboBoxActiveXControl comboBoxControl = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper för ComboBox ActiveX-kontrollen
            comboBoxControl.SpecialEffect = ControlSpecialEffectType.Sunken;
            comboBoxControl.ListWidth = 100;
            comboBoxControl.ListRows = 5;

            // Lägg till en TextBox ActiveX-kontroll
            shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 5, 0, 5, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper för TextBox ActiveX-kontrollen
            textBoxControl.Text = "Example TextBox";
            textBoxControl.SpecialEffect = ControlSpecialEffectType.Bump;

            // Spara arbetsboken
            workbook.Save("ControlSpecialEffectTypeExample.xlsx");
            workbook.Save("ControlSpecialEffectTypeExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


