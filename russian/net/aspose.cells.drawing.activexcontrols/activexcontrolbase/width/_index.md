---
title: "ActiveXControlBase.Width"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControlBase. Получает и задает ширину элемента управления в пунктах"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/width/
---
## ActiveXControlBase.Width property

Получает и задает ширину элемента управления в единицах точек.

```csharp
public virtual double Width { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            ActiveXControlBase control = (ActiveXControlBase)shape.ActiveXControl;

            // Продемонстрировать использование свойства Width
            Console.WriteLine("Original width: " + control.Width);
            control.Width = 150;
            Console.WriteLine("Modified width: " + control.Width);

            workbook.Save("ActiveXControlWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


