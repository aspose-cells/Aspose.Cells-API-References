---
title: "ActiveXControlBase.ForeOleColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControlBase-Eigenschaft. Liest und schreibt die OLE-Farbe des Vordergrunds"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/
---
## ActiveXControlBase.ForeOleColor property

Ruft die OLE-Farbe des Vordergrunds ab und legt sie fest.

```csharp
public virtual int ForeOleColor { get; set; }
```

### Hinweise

Gilt nicht für das Image-Steuerelement.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyForeOleColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein CheckBox ActiveX-Steuerelement mit allen erforderlichen Parametern hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Grundlegende Eigenschaften festlegen
            checkBox.Caption = "Sample CheckBox";
            checkBox.IsAutoSize = true;

            // Demonstrieren Sie die ForeOleColor-Eigenschaft
            checkBox.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            checkBox.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);

            // Speichere die Arbeitsmappe
            workbook.Save("ActiveXControlForeOleColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


