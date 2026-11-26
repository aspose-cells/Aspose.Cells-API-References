---
title: "Cells.EndCellInColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает последнюю ячейку в этом столбце"
type: docs
url: /ru/net/aspose.cells/cells/endcellincolumn/
---
## EndCellInColumn(int) {#endcellincolumn}

Получает последнюю ячейку в этом столбце.

```csharp
public Cell EndCellInColumn(int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | Индекс столбца. |

### Возвращаемое значение

Объект ячейки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodEndCellInColumnWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Получить последнюю ячейку в столбце A (индекс столбца 0)
            Cell lastCell = worksheet.Cells.EndCellInColumn(0);
            
            Console.WriteLine("Last cell in column A: Row " + lastCell.Row + ", Value: " + lastCell.StringValue);

            // Перебрать все строки в столбце A
            for (int row = 0; row <= lastCell.Row; row++)
            {
                Cell cell = worksheet.Cells[row, 0];
                Console.WriteLine("Row " + row + ": " + cell.StringValue);
            }

            // Сохраните книгу
            workbook.Save("EndCellInColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EndCellInColumn(int, int, int, int) {#endcellincolumn_1}

Получает последнюю ячейку с максимальным индексом столбца в этом диапазоне.

```csharp
public Cell EndCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Индекс начальной строки. |
| endRow | Int32 | Индекс конечной строки. |
| startColumn | Int32 | Индекс начального столбца. |
| endColumn | Int32 | Индекс конечного столбца. |

### Возвращаемое значение

Объект ячейки.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить данные в столбце B (индекс 1)
            worksheet.Cells[0, 1].PutValue("Data 1");
            worksheet.Cells[2, 1].PutValue("Data 2");
            worksheet.Cells[3, 1].PutValue("Data 3");

            try
            {
                // Вызвать EndCellInColumn с параметрами: startRow=0, endRow=5, startColumn=1, endColumn=1
                Cell result = worksheet.Cells.EndCellInColumn(0, 5, 1, 1);

                if (result != null)
                {
                    Console.WriteLine($"Last cell in column B between rows 0-5 is at row {result.Row}, column {result.Column}");
                    // Отметить найденную ячейку
                    result.PutValue("Last Cell");
                    Style style = result.GetStyle();
                    style.Font.IsBold = true;
                    result.SetStyle(style);
                }
                else
                {
                    Console.WriteLine("No cells found in specified range");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EndCellInColumn method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


