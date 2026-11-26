---
title: "SpinButtonActiveXControl.SmallChange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "SpinButtonActiveXControl property. Получает и задает величину, на которую изменяется свойство Position"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/smallchange/
---
## SpinButtonActiveXControl.SmallChange property

Получает и задает величину, на которую изменяется свойство Position

```csharp
public int SmallChange { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertySmallChangeDemo
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
            
            // Получите элемент управления ActiveX и задайте свойство SmallChange
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.SmallChange = 5;
            
            // Сохраните книгу
            workbook.Save("SpinButtonSmallChangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


