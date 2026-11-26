---
title: "Cells.GetRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает элемент Row по указанному индексу строки ячейки"
type: docs
url: /ru/net/aspose.cells/cells/getrow/
---
## Cells.GetRow method

Получает элемент [`Row`](../../row/) по указанному индексу строки ячейки.

```csharp
[Obsolete("Use Cells.CheckRow(int row) instead.")]
public Row GetRow(int row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки |

### Возвращаемое значение

Если объект строки существует, возвращает объект Row, иначе возвращает null.

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Cells.CheckRow(int row). Этот метод будет удалён через 12 месяцев, начиная с февраля 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте ячейки в строке 5, чтобы убедиться, что строка существует.
            worksheet.Cells["A5"].PutValue("Row 5 Data");
            worksheet.Cells["B5"].PutValue(12345);

            try
            {
                // Вызовите метод GetRow с параметром Int32.
                Row resultRow = worksheet.Cells.GetRow(5);

                if (resultRow != null)
                {
                    // Продемонстрировать манипуляцию строкой
                    resultRow.Height = 20;
                    Console.WriteLine($"Retrieved row 5 successfully. Current height: {resultRow.Height} points");
                    
                    // Подсчитайте ячейки в строке.
                    int cellCount = 0;
                    foreach (Cell cell in resultRow)
                    {
                        cellCount++;
                    }
                    Console.WriteLine($"Row 5 contains {cellCount} cells");
                }
                else
                {
                    Console.WriteLine("Row 5 not found in worksheet");
                }
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid row index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRow: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("CellsMethodGetRowWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


