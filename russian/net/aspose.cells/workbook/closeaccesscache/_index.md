---
title: "Workbook.CloseAccessCache"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Закрывает сеанс, использующий кэши для доступа к данным"
type: docs
url: /ru/net/aspose.cells/workbook/closeaccesscache/
---
## Workbook.CloseAccessCache method

Закрывает сеанс, использующий кэши для доступа к данным.

```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| opts | AccessCacheOptions | параметры доступа к данным |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные и условное форматирование
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i % 2 == 0 ? "Data" : "Other");
            }

            // Добавить условное форматирование
            int ruleIdx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[ruleIdx];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Equal, "Data", null);
            Style style = workbook.CreateStyle();
            style.Font.Size = 16;
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 9, EndColumn = 0 });
            fcc[0].Style = style;

            // Запустить кэш доступа для условного форматирования
            workbook.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Получить доступ к ячейкам с кэшированным условным форматированием
            for (int i = 0; i < 10; i++)
            {
                Cell cell = cells[i, 0];
                Console.WriteLine($"Cell {cell.Name}: Value={cell.StringValue}, FontSize={cell.GetDisplayStyle().Font.Size}");
            }

            // Закройте кэш доступа
            workbook.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


