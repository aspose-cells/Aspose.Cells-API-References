---
title: "LightCellsDataHandler.StartRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LightCellsDataHandler. Подготавливает обработку строки"
type: docs
url: /ru/net/aspose.cells/lightcellsdatahandler/startrow/
---
## LightCellsDataHandler.StartRow method

Подготавливает обработку строки.

```csharp
public bool StartRow(int rowIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | Int32 | индекс следующей строки для обработки |

### Возвращаемое значение

нужно ли обрабатывать эту строку (свойства или данные ячеек). false — игнорировать эту строку и её ячейки и проверить следующую строку.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodStartRowWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                using (Workbook workbook = new Workbook())
                {
                    Worksheet sheet = workbook.Worksheets[0];
                    for (int i = 0; i < 5; i++)
                    {
                        sheet.Cells[i, 0].Value = $"Row {i + 1}";
                    }
                    workbook.Save("input.xlsx");
                }

                LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
                loadOptions.LightCellsDataHandler = new CustomLightCellsDataHandler();
                
                using (Workbook workbook = new Workbook("input.xlsx", loadOptions))
                {
                    workbook.Save("output.xlsx");
                }

                Console.WriteLine("Method executed successfully. Rows with even indices processed.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartRow: {ex.Message}");
            }
        }

        private class CustomLightCellsDataHandler : LightCellsDataHandler
        {
            public bool StartRow(int rowIndex)
            {
                return rowIndex % 2 == 0;
            }

            public bool StartSheet(Worksheet sheet) => true;
            public bool ProcessRow(Row row) => true;
            public bool StartCell(int columnIndex) => true;
            public bool ProcessCell(Cell cell) => true;
        }
    }
}
```

### См. также

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


