---
title: "ActiveXControlBase.MouseIcon"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ActiveXControlBase özelliği. Kontrol için fare imleci olarak gösterilecek özel bir simgeyi alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/
---
## ActiveXControlBase.MouseIcon property

Kontrol için fare imleci olarak gösterilecek özel bir simgeyi alır ve ayarlar.

```csharp
public byte[] MouseIcon { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


