---
title: "LightCellsDataHandler.ProcessRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LightCellsDataHandler. Начинает обработку одной строки"
type: docs
url: /ru/net/aspose.cells/lightcellsdatahandler/processrow/
---
## LightCellsDataHandler.ProcessRow method

Начинает обработку одной строки.

```csharp
public bool ProcessRow(Row row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Row | Объект строки, который в данный момент обрабатывается. |

### Возвращаемое значение

нужно ли обрабатывать ячейки этой строки. false — игнорировать все ячейки в этой строке.

### Примечания

Будет вызвано после чтения свойств строки, таких как высота, стиль и т.д. Однако ячейки в этой строке ещё не прочитаны.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodProcessRowWithRowDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавьте примерные данные
                worksheet.Cells["A1"].Value = "Test Data";
                worksheet.Cells["A2"].Value = 100;
                worksheet.Cells["B2"].Value = 200;

                // Создать пользовательский обработчик
                var handler = new CustomRowHandler();

                // Обработать первую строку
                Row firstRow = worksheet.Cells.Rows[0];
                bool result = handler.ProcessRow(firstRow);

                Console.WriteLine($"ProcessRow returned: {result}");
                Console.WriteLine($"Row height after processing: {firstRow.Height}");

                workbook.Save("ProcessRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ProcessRow demo: {ex.Message}");
            }
        }

        private class CustomRowHandler : LightCellsDataHandler
        {
            public bool ProcessRow(Row row)
            {
                // Продемонстрировать доступ к свойствам строки
                Console.WriteLine($"Processing row index: {row.Index}");
                Console.WriteLine($"Row is hidden: {row.IsHidden}");
                Console.WriteLine($"Row is blank: {row.IsBlank}");

                // Изменить высоту строки, если это не строка заголовка
                if (row.Index > 0)
                {
                    row.Height = 25.0;
                }

                return true;
            }

            public bool StartSheet(Worksheet sheet) => true;
            public bool StartRow(int rowIndex) => true;
            public bool StartCell(int columnIndex) => true;
            public bool ProcessCell(Cell cell) => true;
        }
    }
}
```

### См. также

* class [Row](../../row/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


