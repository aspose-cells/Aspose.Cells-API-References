---
title: "ActiveXControlBase.MouseIcon"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControlBase-Eigenschaft. Liest und schreibt ein benutzerdefiniertes Icon, das als Mauszeiger für das Steuerelement angezeigt wird"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/
---
## ActiveXControlBase.MouseIcon property

Ruft ein benutzerdefiniertes Symbol ab und legt es fest, das als Mauszeiger für das Steuerelement angezeigt wird.

```csharp
public byte[] MouseIcon { get; set; }
```

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System.IO;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyMouseIconDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 0, 1, 0, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            imageControl.MouseIcon = File.ReadAllBytes("mouse.ico");
            imageControl.MousePointer = ControlMousePointerType.Custom;

            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


