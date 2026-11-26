---
title: "SpinButtonActiveXControl.Max"
second_title: "Справочник API Aspose.Cells для .NET"
description: "SpinButtonActiveXControl property. Получает и задает максимальное допустимое значение"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/
---
## SpinButtonActiveXControl.Max property

Получает и задает максимальное допустимое значение.

```csharp
public int Max { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMaxDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте SpinButton ActiveX control на лист
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 1, 1, 1, 100, 30);
            
            // Получите элемент управления ActiveX и задайте его свойство Max
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Max = 100;
            
            // Сохраните книгу
            workbook.Save("SpinButtonMaxDemo.xlsx");
        }
    }
}
```

### См. также

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


