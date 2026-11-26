---
title: "CheckBox.Shadow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CheckBox. Указывает, имеет ли комбобокс 3D‑тень"
type: docs
url: /ru/net/aspose.cells.drawing/checkbox/shadow/
---
## CheckBox.Shadow property

Указывает, имеет ли комбобокс 3‑D затенение.

```csharp
public bool Shadow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyShadowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте флажок на лист и получите его индекс
            int checkBoxIndex = sheet.CheckBoxes.Add(1, 1, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[checkBoxIndex];
            
            // Настройте свойства флажка
            checkBox.Text = "Enable Feature";
            checkBox.Value = true;
            
            // Продемонстрировать свойство Shadow
            checkBox.Shadow = true; // Enable shadow effect
            workbook.Save("CheckBoxWithShadow.xlsx");
            
            checkBox.Shadow = false; // Disable shadow effect
            workbook.Save("CheckBoxWithoutShadow.xlsx");
        }
    }
}
```

### См. также

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


