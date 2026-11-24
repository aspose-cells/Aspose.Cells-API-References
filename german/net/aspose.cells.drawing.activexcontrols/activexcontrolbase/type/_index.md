---
title: "ActiveXControlBase.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControlBase-Eigenschaft. Gibt den Typ des ActiveX-Steuerelements zurück"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/type/
---
## ActiveXControlBase.Type property

Liest den Typ des ActiveX-Steuerelements.

```csharp
public abstract ControlType Type { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Label ActiveX-Steuerelement mit korrekten Parametern hinzufügen
            Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 100, 50, 0);
            LabelActiveXControl labelControl = (LabelActiveXControl)labelShape.ActiveXControl;
            labelControl.Caption = "Label_ActiveX";

            // Demonstriere die Verwendung der Type‑Eigenschaft
            if (labelShape.ActiveXControl.Type == ControlType.Label)
            {
                Console.WriteLine("The control is a Label type");
                labelControl.Caption = labelControl.Caption.Replace("Label_", "MyChangedLabel_");
            }

            // Speichern und überprüfen
            workbook.Save("output.xlsx");
            Console.WriteLine("Label caption changed to: " + labelControl.Caption);
        }
    }
}
```

### Siehe auch

* enum [ControlType](../../controltype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


