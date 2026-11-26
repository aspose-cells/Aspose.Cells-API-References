---
title: "ActiveXControlBase.MouseIcon"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControlBase. Получает и задает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/
---
## ActiveXControlBase.MouseIcon property

Получает и задает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления.

```csharp
public byte[] MouseIcon { get; set; }
```

### Примеры

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

### См. также

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


