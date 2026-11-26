---
title: "Cells.GetFirstDataRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Возвращает индекс первой строки ячейки, содержащей данные в указанном столбце"
type: docs
url: /ru/net/aspose.cells/cells/getfirstdatarow/
---
## Cells.GetFirstDataRow method

Получает индекс первой строки ячейки, содержащей данные в указанном столбце.

```csharp
public int GetFirstDataRow(int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |

### Возвращаемое значение

индекс первой строки.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetFirstDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте несколько примерных данных, чтобы продемонстрировать метод
            worksheet.Cells["A1"].Value = "Header";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["A3"].Value = "Data2";
            worksheet.Cells["B5"].Value = "Data3";
            worksheet.Cells["C7"].Value = "Data4";

            try
            {
                // Получите коллекцию Cells из листа
                Cells cells = worksheet.Cells;

                // Вызовите GetFirstDataRow для столбца A (индекс 0)
                int firstDataRowA = cells.GetFirstDataRow(0);
                Console.WriteLine($"First data row in column A: {firstDataRowA}");

                // Вызовите GetFirstDataRow для столбца B (индекс 1)
                int firstDataRowB = cells.GetFirstDataRow(1);
                Console.WriteLine($"First data row in column B: {firstDataRowB}");

                // Вызовите GetFirstDataRow для столбца C (индекс 2)
                int firstDataRowC = cells.GetFirstDataRow(2);
                Console.WriteLine($"First data row in column C: {firstDataRowC}");

                // Сохраните книгу
                workbook.Save("GetFirstDataRowDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


