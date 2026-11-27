---
title: "Enum ControlCaptionAlignmentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlCaptionAlignmentType enum. Representerar positionen för rubriken i förhållande till kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/controlcaptionalignmenttype/
---
## ControlCaptionAlignmentType enumeration

Representerar positionen för Caption relativt kontrollen.

```csharp
public enum ControlCaptionAlignmentType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Left | `0` | Vänster sida av kontrollen. |
| Right | `1` | Höger sida av kontrollen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlCaptionAlignmentTypeDemo
    {
        public static void ControlCaptionAlignmentTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en CheckBox ActiveX-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 1, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Ange egenskaper för CheckBoxen
            checkBox.Caption = "Check Me!";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.Checked;

            // Lägg till en RadioButton ActiveX-kontroll i kalkylbladet
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 10, 0, 1, 1, 100, 20);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape2.ActiveXControl;

            // Ange egenskaper för RadioButtonen
            radioButton.Caption = "Select Me!";
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;

            // Spara arbetsboken
            workbook.Save("ControlCaptionAlignmentTypeExample.xlsx");
            workbook.Save("ControlCaptionAlignmentTypeExample.pdf");
            // Skriv ut resultaten
            Console.WriteLine("CheckBox Alignment: " + checkBox.Alignment);
            Console.WriteLine("RadioButton Alignment: " + radioButton.Alignment);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


