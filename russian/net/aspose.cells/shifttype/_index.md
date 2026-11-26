---
title: "Перечисление ShiftType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ShiftType. Представляет варианты сдвига при удалении диапазона ячеек"
type: docs
url: /ru/net/aspose.cells/shifttype/
---
## ShiftType enumeration

Представляет параметры сдвига при удалении диапазона ячеек.

```csharp
public enum ShiftType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Down | `0` | Сдвинуть ячейки вниз. |
| Left | `1` | Сдвинуть ячейки влево. |
| None | `2` | Не сдвигать ячейки. |
| Right | `3` | Сдвинуть ячейки вправо. |
| Up | `4` | Сдвинуть ячейки вверх. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ShiftTypeDemo
    {
        public static void ShiftTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Вставить новую строку с индексом 1, сдвинув существующие строки вниз
            worksheet.Cells.InsertRows(1, 1, true);

            // Установить значение в только что вставленную строку
            worksheet.Cells["A1"].PutValue("New Item");

            // Удалить диапазон ячеек и сдвинуть ячейки вверх
            worksheet.Cells.DeleteRange(2, 0, 2, 1, ShiftType.Up);

            // Вывести оставшиеся значения в первом столбце
            for (int row = 0; row < worksheet.Cells.MaxDataRow + 1; row++)
            {
                Console.WriteLine(worksheet.Cells[row, 0].StringValue);
            }

            // Сохраните книгу
            workbook.Save("ShiftTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


