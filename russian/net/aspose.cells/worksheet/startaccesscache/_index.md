---
title: "Worksheet.StartAccessCache"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Запускает сеанс, использующий кэши для доступа к данным в этом листе"
type: docs
url: /ru/net/aspose.cells/worksheet/startaccesscache/
---
## Worksheet.StartAccessCache method

Запускает сеанс, использующий кэш для доступа к данным в этом листе.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| opts | AccessCacheOptions | параметры доступа к данным |

### Примечания

После завершения доступа к данным, [`CloseAccessCache`](../closeaccesscache/) следует вызвать с теми же параметрами, чтобы очистить все кэши и восстановить обычный режим доступа.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Установить стиль по умолчанию
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;

            // Добавить условное форматирование
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 10, 10));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Font.Size = 16;

            // Заполните некоторыми данными
            Cells cells = sheet.Cells;
            for (int i = 0; i < 10; i++)
            {
                cells[0, i].PutValue("A");
                cells[i, 0].PutValue(i);
            }

            // Запустить кэш доступа для повышения производительности
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Проверить стили
            for (int i = 0; i < 10; i++)
            {
                Console.WriteLine($"Cell[0,{i}] Font Size: {cells[0, i].GetDisplayStyle().Font.Size}");
                Console.WriteLine($"Cell[{i},0] Font Size: {cells[i, 0].GetDisplayStyle().Font.Size}");
            }

            // Закрыть кэш после завершения
            sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
        }
    }
}
```

### См. также

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


