---
title: "ActiveXControl.IsLocked"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControl-Eigenschaft. Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrol/islocked/
---
## ActiveXControl.IsLocked property

Gibt an, ob Daten im Steuerelement für die Bearbeitung gesperrt sind.

```csharp
public bool IsLocked { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Alle Spalten außer der ersten entsperren
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

            // Erste Spalte sperren
            style = sheet.Cells.Columns[0].GetStyle();
            style.IsLocked = true;
            flag = new StyleFlag();
            flag.Locked = true;
            sheet.Cells.Columns[0].ApplyStyle(style, flag);

            // ActiveX-ComboBox-Steuerelement hinzufügen
            Shape comboBoxShape = sheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                5, 0, 5, 0, 100, 20);

            // ActiveX-Steuereigenschaften einschließlich IsLocked festlegen
            ComboBoxActiveXControl comboBox = 
                (ComboBoxActiveXControl)comboBoxShape.ActiveXControl;
            comboBox.IsLocked = false; // Demonstrate IsLocked property
            comboBox.IsVisible = true;
            comboBox.BorderStyle = ControlBorderType.None;

            // Schützen Sie das Arbeitsblatt
            sheet.Protect(ProtectionType.All);

            // Speichere die Arbeitsmappe
            wb.Save("ActiveXControlIsLockedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


