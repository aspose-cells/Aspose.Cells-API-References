---
title: "ActiveXControlBase.LinkedCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControlBase. Получает и задает связанную ячейку"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/
---
## ActiveXControlBase.LinkedCell property

Получает и задает связанную ячейку.

```csharp
public string LinkedCell { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Инициализировать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте SpinButtonActiveXControl на первый лист
            Aspose.Cells.Drawing.Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 
                10, 10, 100, 30, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;

            // Настройте свойства спин‑кнопки
            spinButton.Min = 0;
            spinButton.Max = 100;
            spinButton.Position = 50;
            spinButton.SmallChange = 1;

            // Свяжите элемент управления с ячейкой A1
            spinButton.LinkedCell = "A1";

            // Установите значение ячейки A1, соответствующее начальной позиции
            workbook.Worksheets[0].Cells["A1"].PutValue(spinButton.Position);

            // Сохраните книгу
            workbook.Save("LinkedCellDemo.xlsx");
        }
    }
}
```

### См. также

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


