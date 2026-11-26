---
title: "Класс CellWatch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CellWatch. Представляет элемент наблюдения за ячейкой в окне наблюдения"
type: docs
url: /ru/net/aspose.cells/cellwatch/
---
## CellWatch class

Представляет элемент наблюдения за ячейкой в 'watch window'.

```csharp
public class CellWatch
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CellWatch](cellwatch/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CellName](../../aspose.cells/cellwatch/cellname/) { get; set; } | Получает и задает имя ячейки. |
| [Column](../../aspose.cells/cellwatch/column/) { get; set; } | Получает и задает столбец ячейки. |
| [Row](../../aspose.cells/cellwatch/row/) { get; set; } | Получает и задает строку ячейки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchDemo
    {
        public static void CellWatchExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            // Получить первый Worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить элемент наблюдения за ячейкой в окно наблюдения
            int watchIndex = sheet.CellWatches.Add("B2");

            // Получить объект CellWatch
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Установка свойств
            cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
            cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
            cellWatch.CellName = "B2";

            // Сохраните книгу
            workbook.Save("CellWatchExample.xlsx");
            workbook.Save("CellWatchExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


