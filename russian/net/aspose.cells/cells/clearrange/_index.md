---
title: "Cells.ClearRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Очищает содержимое и форматирование диапазона"
type: docs
url: /ru/net/aspose.cells/cells/clearrange/
---
## ClearRange(CellArea) {#clearrange}

Очищает содержимое и форматирование диапазона.

```csharp
public void ClearRange(CellArea range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | CellArea | Диапазон для очистки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните ячейки примерными данными
            for (int row = 0; row <= 2; row++)
            {
                for (int col = 0; col <= 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data_{row}_{col}";
                }
            }

            // Определите CellArea для очистки (строки 0-2, столбцы 0-2)
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 0;
            clearArea.EndRow = 2;
            clearArea.StartColumn = 0;
            clearArea.EndColumn = 2;

            try
            {
                // Очистить указанный диапазон
                worksheet.Cells.ClearRange(clearArea);
                Console.WriteLine("Cleared cells in range: Rows 0-2, Columns 0-2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearRange method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("CellsMethodClearRangeWithCellAreaDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearRange(int, int, int, int) {#clearrange_1}

Очищает содержимое и форматирование диапазона.

```csharp
public void ClearRange(int startRow, int startColumn, int endRow, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Индекс начальной строки. |
| startColumn | Int32 | Индекс начального столбца. |
| endRow | Int32 | Индекс конечной строки. |
| endColumn | Int32 | Индекс конечного столбца. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Заполнить некоторыми тестовыми данными
            cells[0, 0].PutValue(1);
            cells[0, 16383].PutValue(2);
            cells[1048575, 0].PutValue(3);
            cells[1048575, 16383].PutValue(4);

            // Очистить весь диапазон листа
            cells.ClearRange(0, 0, 1048575, 16383);

            // Сохраните книгу
            workbook.Save("ClearRangeDemo.xlsx");

            Console.WriteLine("ClearRange demo executed successfully.");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


