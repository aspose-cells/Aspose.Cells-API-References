---
title: "CheckBoxActiveXControl.GroupName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CheckBoxActiveXControl. Получает и задает имя группы"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/groupname/
---
## CheckBoxActiveXControl.GroupName property

Получает и задает имя группы.

```csharp
public string GroupName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления CheckBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Установите свойство GroupName
            checkBox.GroupName = "Sheet1";

            // Проверьте и выведите значение GroupName
            Console.WriteLine("CheckBox GroupName: " + checkBox.GroupName);

            // Сохраните книгу
            workbook.Save("CheckBoxActiveXControlGroupNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


