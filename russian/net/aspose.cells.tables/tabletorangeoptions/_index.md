---
title: "Класс TableToRangeOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Tables.TableToRangeOptions. Представляет параметры при преобразовании таблицы в диапазон"
type: docs
url: /ru/net/aspose.cells.tables/tabletorangeoptions/
---
## TableToRangeOptions class

Представляет параметры при преобразовании таблицы в диапазон.

```csharp
public class TableToRangeOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TableToRangeOptions](tabletorangeoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [LastRow](../../aspose.cells.tables/tabletorangeoptions/lastrow/) { get; set; } | Получает и задает индекс последней строки таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableToRangeOptionsDemo
    {
        public static void TableToRangeOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполните лист некоторыми данными
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Добавить объект ListObject (таблицу) в лист
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Установите некоторые свойства таблицы
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;

            // Создайте экземпляр TableToRangeOptions
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 9 // Set the last row index of the table
            };

            // Преобразуйте таблицу в диапазон, используя параметры
            table.ConvertToRange(options);

            // Сохраните книгу
            workbook.Save("TableToRangeOptionsExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


