---
title: "ActiveXControl.IsTransparent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControl. Указывает, является ли элемент управления прозрачным"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/
---
## ActiveXControl.IsTransparent property

Указывает, является ли элемент управления прозрачным.

```csharp
public bool IsTransparent { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsTransparentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для размещения элемента управления ActiveX со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 200, 50, 
                0, 0); // Adding missing parameters for upperLeftRow, upperLeftColumn, height, width, left, top

            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Установить свойства элемента управления
            label.Caption = "Sample Label";
            label.IsTransparent = false; // Demonstrating IsTransparent property

            // Проверить и вывести свойство IsTransparent
            Console.WriteLine("Label IsTransparent property: " + label.IsTransparent);

            // Изменить прозрачность и снова проверить
            label.IsTransparent = true;
            Console.WriteLine("Label IsTransparent property after change: " + label.IsTransparent);

            // Сохраните книгу
            workbook.Save("ActiveXControlIsTransparentDemo.xlsx");
        }
    }
}
```

### См. также

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


