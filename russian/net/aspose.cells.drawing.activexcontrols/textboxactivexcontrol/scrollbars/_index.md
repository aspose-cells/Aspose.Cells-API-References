---
title: "TextBoxActiveXControl.ScrollBars"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Указывает, имеет ли элемент управления вертикальные полосы прокрутки, горизонтальные, обе или ни одной"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scrollbars/
---
## TextBoxActiveXControl.ScrollBars property

Указывает, имеет ли элемент управления вертикальные полосы прокрутки, горизонтальные, обе или ни одну.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать новую коллекцию фигур и добавить ActiveX‑контрол
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
            
            // Установить свойство ScrollBars в vertical
            textBox.ScrollBars = ControlScrollBarType.BarsVertical;
            
            // Сохраните книгу
            workbook.Save("TextBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


