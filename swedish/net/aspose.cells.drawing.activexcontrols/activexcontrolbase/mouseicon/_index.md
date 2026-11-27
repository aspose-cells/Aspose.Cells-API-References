---
title: "ActiveXControlBase.MouseIcon"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Hämtar och anger en anpassad ikon som ska visas som muspekare för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/
---
## ActiveXControlBase.MouseIcon property

Hämtar och anger en anpassad ikon som ska visas som muspekare för kontrollen.

```csharp
public byte[] MouseIcon { get; set; }
```

### Exempel

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

### Se även

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


