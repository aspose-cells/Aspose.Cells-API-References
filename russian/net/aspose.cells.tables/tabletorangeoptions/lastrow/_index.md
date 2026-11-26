---
title: "TableToRangeOptions.LastRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TableToRangeOptions. Получает и задает индекс последней строки таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tabletorangeoptions/lastrow/
---
## TableToRangeOptions.LastRow property

Получает и задает индекс последней строки таблицы.

```csharp
public int LastRow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableToRangeOptionsPropertyLastRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать примерные данные
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"Data {row}-{col}");
                }
            }

            // Создайте таблицу
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // Преобразовать таблицу в диапазон с указанным параметром LastRow
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 7 // Only convert rows 0-7 (excluding 8-9)
            };
            table.ConvertToRange(options);

            workbook.Save("TableToRangeWithLastRow.xlsx");
        }
    }
}
```

### См. также

* class [TableToRangeOptions](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


