---
title: "Cells.GetGroupedRowOutlineLevel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает уровень контуров строки, отсчитываемый с нуля"
type: docs
url: /ru/net/aspose.cells/cells/getgroupedrowoutlinelevel/
---
## Cells.GetGroupedRowOutlineLevel method

Получает уровень структуры (нумерация с нуля) строки.

```csharp
public int GetGroupedRowOutlineLevel(int rowIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | Индекс строки. |

### Возвращаемое значение

Уровень контуров (отсчитываемый с нуля) строки.

### Примечания

Если строка не сгруппирована, возвращает ноль.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedRowOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Сгруппировать строки 0-3 (уровень 1)
            cells.GroupRows(0, 3, false);
            
            // Сгруппировать строки 0-1 (уровень 2)
            cells.GroupRows(0, 1, false);

            // Получить уровень контуров для каждой строки
            for (int row = 0; row <= 4; row++)
            {
                int outlineLevel = cells.GetGroupedRowOutlineLevel(row);
                Console.WriteLine($"Row {row} outline level: {outlineLevel}");
            }

            // Разгруппировать все строки
            cells.UngroupRows(0, 3);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


