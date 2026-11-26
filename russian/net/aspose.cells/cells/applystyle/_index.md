---
title: "Cells.ApplyStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Применяет форматы ко всему листу"
type: docs
url: /ru/net/aspose.cells/cells/applystyle/
---
## Cells.ApplyStyle method

Применяет форматы ко всему листу.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | Объект стиля, который будет применён. |
| флаг | StyleFlag | Флаги, указывающие применённые свойства форматирования. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = wb.Worksheets[0];
            
            // Создать стиль и включить перенос текста
            Style style = wb.CreateStyle();
            style.IsTextWrapped = true;
            
            // Создать флаг стиля и включить флаг переноса текста
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Применить стиль ко всем ячейкам листа
            sheet.Cells.ApplyStyle(style, flag);
            
            // Сохраните книгу
            wb.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


