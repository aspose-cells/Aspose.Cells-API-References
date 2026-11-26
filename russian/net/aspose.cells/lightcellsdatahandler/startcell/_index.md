---
title: "LightCellsDataHandler.StartCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LightCellsDataHandler. Подготавливает обработку ячейки"
type: docs
url: /ru/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

Подготавливает обработку ячейки.

```csharp
public bool StartCell(int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | индекс столбца ячейки, которую нужно обработать |

### Возвращаемое значение

нужно ли обрабатывать эту ячейку. false — игнорировать ячейку и проверить следующую, пока не достигнут конец данных ячеек текущей строки

### Примечания

Будет вызвано при достижении существующей ячейки в текущей строке. Текущая строка — это строка последнего вызова [`ProcessRow`](../processrow/).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodStartCellWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Создать временный входной файл
                File.WriteAllText("input.csv", "Column1,Column2,Column3\n1,2,3\n4,5,6");

                // Создать параметры загрузки с пользовательским обработчиком LightCells
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Загрузить книгу с пользовательским обработчиком
                Workbook workbook = new Workbook("input.csv", loadOptions);

                // Сохранить обработанную книгу
                workbook.Save("output.xlsx");
                Console.WriteLine("StartCell method executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartCell method: {ex.Message}");
            }
        }

        private class CustomLightCellsDataHandler : LightCellsDataHandler
        {
            public bool StartSheet(Worksheet sheet)
            {
                return true; // Process all sheets
            }

            public bool StartRow(int rowIndex)
            {
                return true; // Process all rows
            }

            public bool StartCell(int columnIndex)
            {
                // Обрабатывать только ячейки в столбце с индексом 1 (второй столбец)
                return columnIndex == 1;
            }

            public bool ProcessCell(Cell cell)
            {
                // Удвоить значение ячеек во втором столбце
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                return true;
            }

            public bool ProcessRow(Row row)
            {
                return true; // Continue processing
            }
        }
    }
}
```

### См. также

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


