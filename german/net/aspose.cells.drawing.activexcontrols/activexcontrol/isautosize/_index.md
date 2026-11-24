---
title: "ActiveXControl.IsAutoSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControl-Eigenschaft. Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/
---
## ActiveXControl.IsAutoSize property

Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen.

```csharp
public virtual bool IsAutoSize { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Korrigierte AddActiveXControl-Parameter mit vollständiger Signatur
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 0, 0, 100, 50);
            ActiveXControl control = shape.ActiveXControl;

            Console.WriteLine("Initial IsAutoSize: " + control.IsAutoSize);
            control.IsAutoSize = true;
            Console.WriteLine("Set IsAutoSize: " + control.IsAutoSize);

            string outputPath = "AutoSizeControlDemo.xlsm";
            workbook.Save(outputPath, SaveFormat.Xlsm);

            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ActiveXControl loadedControl = loadedShape.ActiveXControl;
            Console.WriteLine("Loaded IsAutoSize: " + loadedControl.IsAutoSize);
        }
    }
}
```

### Siehe auch

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


