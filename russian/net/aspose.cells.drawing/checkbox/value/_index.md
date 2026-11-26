---
title: "CheckBox.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CheckBox. Указывает, отмечен ли флажок"
type: docs
url: /ru/net/aspose.cells.drawing/checkbox/value/
---
## CheckBox.Value property

Указывает, отмечен ли флажок или нет.

```csharp
public bool Value { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int checkBoxIndex = sheet.CheckBoxes.Add(0, 0, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[checkBoxIndex];
            checkBox.Value = true;
            checkBox.Text = "Sample Checkbox";

            workbook.Save("CheckBoxValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


