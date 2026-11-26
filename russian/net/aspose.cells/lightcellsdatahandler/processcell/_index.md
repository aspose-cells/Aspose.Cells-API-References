---
title: "LightCellsDataHandler.ProcessCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LightCellsDataHandler. Начинает обработку одной ячейки"
type: docs
url: /ru/net/aspose.cells/lightcellsdatahandler/processcell/
---
## LightCellsDataHandler.ProcessCell method

Начинает обработку одной ячейки.

```csharp
public bool ProcessCell(Cell cell)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ячейка | Ячейка | Объект Cell, который в данный момент обрабатывается |

### Возвращаемое значение

нужно ли сохранять эту ячейку в модели ячеек текущего листа. Обычно это должно быть false, чтобы после обработки ячейки не удерживались в памяти и память освобождалась. Для некоторых специальных целей, например когда пользователю необходимо позже получить доступ к некоторым ячейкам после полной обработки книги, пользователь может заставить этот метод вернуть true, чтобы такие специальные ячейки оставались в модели Cells и к ним можно было обратиться позже через API, такие как Cells[row, column]. Однако хранение данных ячеек в модели Cells требует больше памяти, и если сохраняются все ячейки, чтение шаблонного файла в режиме LightCells будет таким же, как чтение обычным способом.

### Примечания

Будет вызвано после чтения данных одной ячейки.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodProcessCellWithCellDemo
    {
        public static void Run()
        {
            try
            {
                // Создать временный файл данных
                File.WriteAllText("input.txt", "A,B,C\n10,20,30\n40,50,60");

                // Создать параметры загрузки с пользовательским обработчиком LightCells
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Загрузить книгу с пользовательским обработчиком
                Workbook workbook = new Workbook("input.txt", loadOptions);

                // Сохранить обработанные результаты
                workbook.Save("output.xlsx");
                Console.WriteLine("ProcessCell executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ProcessCell: {ex.Message}");
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
                return true; // Process all cells
            }

            public bool ProcessCell(Cell cell)
            {
                // Удвоить числовые значения и пометить строки
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                else if (cell.Type == CellValueType.IsString)
                {
                    cell.PutValue($"TEXT: {cell.StringValue}");
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

* class [Cell](../../cell/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


