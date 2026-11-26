---
title: "LightCellsDataHandler.StartSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LightCellsDataHandler. Начинает обработку листа"
type: docs
url: /ru/net/aspose.cells/lightcellsdatahandler/startsheet/
---
## LightCellsDataHandler.StartSheet method

Начинает обработку рабочего листа.

```csharp
public bool StartSheet(Worksheet sheet)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| лист | Worksheet | рабочий лист для чтения данных ячеек. |

### Возвращаемое значение

нужно ли обрабатывать данные ячеек этого листа. false — игнорировать этот лист.

### Примечания

Будет вызвано перед чтением данных ячеек рабочего листа.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodStartSheetWithWorksheetDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                CustomLightCellsDataHandler handler = new CustomLightCellsDataHandler();
                bool result = handler.StartSheet(worksheet);

                Console.WriteLine($"StartSheet method returned: {result}");
                Console.WriteLine($"Worksheet name after StartSheet: {worksheet.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }

            workbook.Save("LightCellsDataHandlerStartSheetDemo.xlsx");
        }
    }

    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet)
        {
            sheet.Name = "ModifiedByStartSheet";
            return true;
        }

        public bool StartRow(int rowIndex) => true;
        public bool ProcessRow(Row row) => true;
        public bool StartCell(int columnIndex) => true;
        public bool ProcessCell(Cell cell) => true;
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


