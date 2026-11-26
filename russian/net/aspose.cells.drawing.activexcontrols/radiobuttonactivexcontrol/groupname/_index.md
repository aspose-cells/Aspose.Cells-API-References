---
title: "RadioButtonActiveXControl.GroupName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RadioButtonActiveXControl. Получает и задает имя группы"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/groupname/
---
## RadioButtonActiveXControl.GroupName property

Получает и задает имя группы.

```csharp
public string GroupName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить два RadioButton ActiveX контрола
            var shape1 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 30);
            var radio1 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape1.ActiveXControl;
            
            var shape2 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 50, 100, 30);
            var radio2 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape2.ActiveXControl;

            // Установите одинаковое имя группы, чтобы сделать их взаимно исключающимися
            radio1.GroupName = "RadioGroup1";
            radio2.GroupName = "RadioGroup1";

            // Установить подписи
            radio1.Caption = "Option 1";
            radio2.Caption = "Option 2";

            // Сохраните книгу
            workbook.Save("RadioButtonGroupDemo.xlsx");
        }
    }
}
```

### См. также

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


