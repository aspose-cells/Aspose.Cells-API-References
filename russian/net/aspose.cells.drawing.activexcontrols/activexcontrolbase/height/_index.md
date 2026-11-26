---
title: "ActiveXControlBase.Height"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ActiveXControlBase. Получает и задает высоту контролла в пунктах"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/height/
---
## ActiveXControlBase.Height property

Получает и задает высоту элемента управления в единицах точек.

```csharp
public virtual double Height { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyHeightDemo
    {
        public static void Run()
        {
            // Инициализировать новую книгу
            Workbook workbook = new Workbook();

            // Добавьте RadioButton ActiveXControl
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 50);
            RadioButtonActiveXControl activeXControl = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Установите базовые свойства
            activeXControl.Caption = "Height Demo";
            activeXControl.IsAutoSize = false; // Disable auto-size to demonstrate Height property

            // Продемонстрировать свойство Height
            Console.WriteLine("Original Height: " + activeXControl.Height);
            activeXControl.Height = 75;
            Console.WriteLine("Modified Height: " + activeXControl.Height);

            // Сохраните книгу
            workbook.Save("ActiveXControlHeightDemo.xlsx");
        }
    }
}
```

### См. также

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


