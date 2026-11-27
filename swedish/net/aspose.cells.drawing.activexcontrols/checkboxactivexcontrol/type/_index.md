---
title: "CheckBoxActiveXControl.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxActiveXControl egenskap. Hämtar typen av ActiveX‑kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/type/
---
## CheckBoxActiveXControl.Type property

Hämtar typen av ActiveX-kontrollen.

```csharp
public override ControlType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en CheckBox ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper
            checkBox.Caption = "Sample CheckBox";
            checkBox.GroupName = "Sheet1";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.UnChecked;
            checkBox.IsEnabled = true;

            // Demonstrera användning av Type-egenskapen
            Console.WriteLine("Control Type: " + checkBox.Type); // Output: Control Type: CheckBox
            if (checkBox.Type == ControlType.CheckBox)
            {
                Console.WriteLine("This is a CheckBox control");
            }

            // Spara arbetsboken
            workbook.Save("CheckBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlType](../../controltype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


