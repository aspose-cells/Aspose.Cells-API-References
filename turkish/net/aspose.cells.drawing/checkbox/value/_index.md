---
title: "CheckBox.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CheckBox özelliği. Onay kutusunun işaretli olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/checkbox/value/
---
## CheckBox.Value property

Onay kutusunun işaretli olup olmadığını gösterir.

```csharp
public bool Value { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


