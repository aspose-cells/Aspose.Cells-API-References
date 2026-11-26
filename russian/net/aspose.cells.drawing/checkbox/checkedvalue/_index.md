---
title: "CheckBox.CheckedValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CheckBox. Получает или задает значение флажка"
type: docs
url: /ru/net/aspose.cells.drawing/checkbox/checkedvalue/
---
## CheckBox.CheckedValue property

Получает или задает значение флажка.

```csharp
public CheckValueType CheckedValue { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyCheckedValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить флажок на лист
            CheckBox checkBox = sheet.Shapes.AddCheckBox(1, 1, 100, 100, 20, 20);

            // Установите значение флажка в Checked
            checkBox.CheckedValue = CheckValueType.Checked;

            // Сохраните книгу
            workbook.Save("CheckBoxCheckedValueDemo.xlsx");

            // Загрузите сохранённую книгу для проверки
            Workbook loadedWorkbook = new Workbook("CheckBoxCheckedValueDemo.xlsx");
            CheckBox loadedCheckBox = (CheckBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Выведите состояние флажка
            Console.WriteLine("CheckBox CheckedValue: " + loadedCheckBox.CheckedValue);
        }
    }
}
```

### См. также

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


