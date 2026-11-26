---
title: "CellsHelper.CellNameToIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Получает индексы строки и столбца ячейки согласно её имени"
type: docs
url: /ru/net/aspose.cells/cellshelper/cellnametoindex/
---
## CellsHelper.CellNameToIndex method

Получает индексы строки и столбца ячейки в соответствии с её именем.

```csharp
public static void CellNameToIndex(string cellName, out int row, out int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |
| строка | Int32& | Индекс строки вывода |
| column | Int32& | Индекс столбца вывода |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodCellNameToIndexWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Инициализируйте переменные для хранения индексов строки и столбца
            int rowIndex = -1;
            int columnIndex = -1;
            string cellName = "C5";

            try
            {
                // Вызовите метод CellNameToIndex, чтобы преобразовать имя ячейки в индексы строки и столбца
                CellsHelper.CellNameToIndex(cellName, out rowIndex, out columnIndex);

                // Отобразите результаты
                Console.WriteLine($"Cell name: {cellName}");
                Console.WriteLine($"Row index: {rowIndex}");
                Console.WriteLine($"Column index: {columnIndex}");

                // Создайте книгу и продемонстрируйте использование индексов
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Получите доступ к ячейке, используя полученные индексы
                Cell cell = worksheet.Cells[rowIndex, columnIndex];
                cell.PutValue("Test Value");

                // Сохраните книгу
                workbook.Save("CellNameToIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CellNameToIndex method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


