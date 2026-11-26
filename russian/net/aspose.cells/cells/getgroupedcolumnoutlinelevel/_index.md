---
title: "Cells.GetGroupedColumnOutlineLevel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает уровень контуров столбца (нумерация с нуля)"
type: docs
url: /ru/net/aspose.cells/cells/getgroupedcolumnoutlinelevel/
---
## Cells.GetGroupedColumnOutlineLevel method

Получает уровень структуры (нумерация с нуля) столбца.

```csharp
public int GetGroupedColumnOutlineLevel(int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс столбца |

### Возвращаемое значение

Уровень контуров столбца

### Примечания

Если столбец не сгруппирован, возвращает ноль.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedColumnOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Группировать столбцы (первые 3 столбца), не скрывая их
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Получить уровень структуры первого столбца
            int outlineLevel = worksheet.Cells.GetGroupedColumnOutlineLevel(0);
            
            Console.WriteLine("Outline level of column 0: " + outlineLevel);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


