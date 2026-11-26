---
title: "Cells.GetCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает элемент Cell или null по указанному индексу строки и столбца ячейки"
type: docs
url: /ru/net/aspose.cells/cells/getcell/
---
## Cells.GetCell method

Получает элемент [`Cell`](../../cell/) или null по указанному индексу строки и столбца ячейки.

```csharp
[Obsolete("Use Cells.CheckCell(int row, int column) instead.")]
public Cell GetCell(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки |
| column | Int32 | Индекс столбца |

### Возвращаемое значение

Возвращает объект Cell, если он существует. Возвращает null, если ячейка не существует.

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод CheckCell(int row, int column). Этот метод будет удалён через 12 месяцев, начиная с февраля 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к ячейке в строке 1, столбце 2 (индекс с нуля)
            Cell cell = worksheet.Cells.GetCell(1, 2);
            
            // Установить значение и стиль для демонстрации
            cell.PutValue("Test Value");
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("GetCellDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


