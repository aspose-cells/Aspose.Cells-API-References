---
title: "Worksheet.GetFreezedPanes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Получает замороженные области"
type: docs
url: /ru/net/aspose.cells/worksheet/getfreezedpanes/
---
## Worksheet.GetFreezedPanes method

Получает замороженные области.

```csharp
public bool GetFreezedPanes(out int row, out int column, out int freezedRows, 
    out int freezedColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32& | Индекс строки. |
| column | Int32& | Индекс столбца. |
| freezedRows | Int32& | Количество видимых строк в верхней области, не более индекса строки. |
| freezedColumns | Int32& | Количество видимых столбцов в левой области, не более индекса столбца. |

### Возвращаемое значение

Возвращает, заморожен ли лист

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodGetFreezedPanesWithInt32ParametersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заморозить области в ячейке C5 (строка 4, столбец 2) с 2 замороженными строками и 1 замороженным столбцом
            worksheet.FreezePanes(4, 2, 2, 1);

            // Объявить переменные для хранения информации о замороженных областях
            int row = 0;
            int column = 0;
            int freezedRows = 0;
            int freezedColumns = 0;

            try
            {
                // Вызвать метод GetFreezedPanes с выходными параметрами
                bool hasFreeze = worksheet.GetFreezedPanes(out row, out column, out freezedRows, out freezedColumns);

                // Отобразите результаты
                Console.WriteLine("Worksheet has freeze panes: " + hasFreeze);
                if (hasFreeze)
                {
                    Console.WriteLine("Freeze position - Row: " + row + ", Column: " + column);
                    Console.WriteLine("Frozen rows: " + freezedRows + ", Frozen columns: " + freezedColumns);
                }

                // Сохраните книгу
                workbook.Save("WorksheetMethodGetFreezedPanesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFreezedPanes method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


