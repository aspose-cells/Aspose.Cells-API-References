---
title: "ScrollBarActiveXControl.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScrollBarActiveXControl. Получает тип элемента управления ActiveX"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type/
---
## ScrollBarActiveXControl.Type property

Получает тип ActiveX‑элемента управления.

```csharp
public override ControlType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ScrollBarActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ScrollBar ActiveX с правильными параметрами
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 1, 1, 100, 20, 0);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Проверьте тип элемента управления, используя свойство Type
            if (scrollBar.Type == ControlType.ScrollBar)
            {
                // Установите специфические свойства ScrollBar
                scrollBar.Max = 100;
                scrollBar.Min = 0;
                scrollBar.Position = 50;
            }

            // Сохраните книгу
            workbook.Save("ScrollBarActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlType](../../controltype/)
* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


