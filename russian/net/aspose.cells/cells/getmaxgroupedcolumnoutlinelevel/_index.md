---
title: "Cells.GetMaxGroupedColumnOutlineLevel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает максимальный уровень группировки столбцов, нумерация с нуля"
type: docs
url: /ru/net/aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/
---
## Cells.GetMaxGroupedColumnOutlineLevel method

Получает максимальный уровень структуры сгруппированных столбцов (нумерация с нуля).

```csharp
public int GetMaxGroupedColumnOutlineLevel()
```

### Возвращаемое значение

Максимальный уровень группировки столбцов (нумерация с нуля)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedColumnOutlineLevelDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Сгруппировать несколько столбцов для демонстрации уровней группировки
            cells.GroupColumns(0, 2, false);
            cells.GroupColumns(3, 5, false);
            
            // Получить максимальный уровень группировки столбцов
            int maxOutlineLevel = cells.GetMaxGroupedColumnOutlineLevel();
            
            Console.WriteLine("Maximum grouped column outline level: " + maxOutlineLevel);
            
            // Отобразить уровень группировки для каждого столбца
            for (int col = 0; col < 6; col++)
            {
                int outlineLevel = cells.GetGroupedColumnOutlineLevel(col);
                Console.WriteLine($"Column {col} outline level: {outlineLevel}");
            }
            
            // Сохраните книгу
            workbook.Save("GroupedColumnsOutlineLevel.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


