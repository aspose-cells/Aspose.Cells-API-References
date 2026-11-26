---
title: "Cells.GetMaxGroupedRowOutlineLevel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает максимальный уровень контуров сгруппированных строк, нулевой базовой"
type: docs
url: /ru/net/aspose.cells/cells/getmaxgroupedrowoutlinelevel/
---
## Cells.GetMaxGroupedRowOutlineLevel method

Получает максимальный уровень структуры сгруппированных строк (нумерация с нуля).

```csharp
public int GetMaxGroupedRowOutlineLevel()
```

### Возвращаемое значение

Максимальный уровень контуров сгруппированных строк (ноль‑базовый)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedRowOutlineLevelDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Сгруппируйте несколько строк, чтобы продемонстрировать уровни контуров
            cells.GroupRows(0, 2, false);
            cells.GroupRows(4, 6, false);
            
            // Добавьте вложенную группировку
            cells.GroupRows(4, 5, true);

            // Получить максимальный уровень контуров сгруппированных строк
            int maxOutlineLevel = cells.GetMaxGroupedRowOutlineLevel();

            // Отобразить результат
            Console.WriteLine("Maximum grouped row outline level: " + maxOutlineLevel);

            // Отобразить уровень контура для каждой строки
            for (int row = 0; row <= 6; row++)
            {
                Console.WriteLine($"Row {row} outline level: {cells.GetGroupedRowOutlineLevel(row)}");
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


