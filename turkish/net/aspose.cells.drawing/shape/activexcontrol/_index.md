---
title: "Shape.ActiveXControl"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. ActiveX denetimini alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/activexcontrol/
---
## Shape.ActiveXControl property

ActiveX denetimini alır.

```csharp
public ActiveXControl ActiveXControl { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ShapePropertyActiveXControlDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 0, 0, 0, 0, 100, 30);

            if (shape.ActiveXControl != null)
            {
                CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
                string fontName = checkBox.Font.Name;
                Console.WriteLine($"CheckBox Font: {fontName}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ActiveXControl](../../../aspose.cells.drawing.activexcontrols/activexcontrol/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


