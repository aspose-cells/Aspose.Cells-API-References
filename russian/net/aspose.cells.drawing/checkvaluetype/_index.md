---
title: "Перечисление CheckValueType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.CheckValueType. Представляет тип значения флажка"
type: docs
url: /ru/net/aspose.cells.drawing/checkvaluetype/
---
## CheckValueType enumeration

Представляет тип значения флажка в элементе управления чекбокс.

```csharp
public enum CheckValueType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| UnChecked | `0` | Не отмечено |
| Checked | `1` | Отмечено |
| Mixed | `2` | Смешанный |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassCheckValueTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить флажки на лист
            int checkboxIndex1 = sheet.CheckBoxes.Add(0, 0, 100, 100);
            int checkboxIndex2 = sheet.CheckBoxes.Add(0, 1, 100, 100);

            // Получить флажки и установить их свойства
            Aspose.Cells.Drawing.CheckBox checkbox1 = sheet.CheckBoxes[checkboxIndex1];
            Aspose.Cells.Drawing.CheckBox checkbox2 = sheet.CheckBoxes[checkboxIndex2];

            // Установить значения флажков и их состояние
            checkbox1.Value = true;
            checkbox1.CheckedValue = CheckValueType.Checked;
            
            checkbox2.Value = false;
            checkbox2.CheckedValue = CheckValueType.UnChecked;  // Note: Changed from Unchecked to UnChecked

            // Связать флажки с ячейками
            checkbox1.LinkedCell = "A1";
            checkbox2.LinkedCell = "A2";

            // Вывести значения ячеек, чтобы продемонстрировать связь
            Console.WriteLine("Cell A1 value (should be true): " + sheet.Cells["A1"].BoolValue);
            Console.WriteLine("Cell A2 value (should be false): " + sheet.Cells["A2"].BoolValue);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


