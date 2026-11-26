---
title: "SpinButtonActiveXControl.Min"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SpinButtonActiveXControl. Получает и задает минимально допустимое значение"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/
---
## SpinButtonActiveXControl.Min property

Получает и задает минимальное допустимое значение.

```csharp
public int Min { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMinDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте SpinButton ActiveX control на лист
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Установите свойство Min у SpinButton
            spinButton.Min = 0;
            
            // Установите другие свойства для демонстрации функциональности
            spinButton.Max = 100;
            spinButton.Position = 50;
            
            // Сохраните книгу
            workbook.Save("SpinButtonMinDemo.xlsx");
        }
    }
}
```

### См. также

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


