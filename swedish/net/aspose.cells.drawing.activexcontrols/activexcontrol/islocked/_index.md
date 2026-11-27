---
title: "ActiveXControl.IsLocked"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControl-egenskap. Anger om data i kontrollen är låst för redigering"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrol/islocked/
---
## ActiveXControl.IsLocked property

Anger om data i kontrollen är låst för redigering.

```csharp
public bool IsLocked { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsLockedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Lås upp alla kolumner förutom den första
            Style style;
            StyleFlag flag;
            for (int i = 0; i <= 255; i++)
            {
                style = sheet.Cells.Columns[(byte)i].GetStyle();
                style.IsLocked = false;
                flag = new StyleFlag();
                flag.Locked = true;
                sheet.Cells.Columns[(byte)i].ApplyStyle(style, flag);
            }

            // Lås den första kolumnen
            style = sheet.Cells.Columns[0].GetStyle();
            style.IsLocked = true;
            flag = new StyleFlag();
            flag.Locked = true;
            sheet.Cells.Columns[0].ApplyStyle(style, flag);

            // Lägg till ActiveX ComboBox-kontroll
            Shape comboBoxShape = sheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                5, 0, 5, 0, 100, 20);

            // Ställ in egenskaper för ActiveX-kontroll inklusive IsLocked
            ComboBoxActiveXControl comboBox = 
                (ComboBoxActiveXControl)comboBoxShape.ActiveXControl;
            comboBox.IsLocked = false; // Demonstrate IsLocked property
            comboBox.IsVisible = true;
            comboBox.BorderStyle = ControlBorderType.None;

            // Skydda kalkylbladet
            sheet.Protect(ProtectionType.All);

            // Spara arbetsboken
            wb.Save("ActiveXControlIsLockedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


