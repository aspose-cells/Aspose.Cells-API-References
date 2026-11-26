---
title: "Worksheet.CloseAccessCache"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Закрывает сеанс, который использует кэши для доступа к данным в этом листе"
type: docs
url: /ru/net/aspose.cells/worksheet/closeaccesscache/
---
## Worksheet.CloseAccessCache method

Закрывает сеанс, использующий кэш для доступа к данным в этом листе.

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
    public class WorksheetMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Заполните ячейки примерными данными
            for (int i = 0; i < 1000; i++)
            {
                cells[i, 0].PutValue(i % 10);
            }

            // Добавить условное форматирование
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 999, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Включите кэш доступа для условного форматирования
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Выполняйте операции с кэшированным доступом
            Random random = new Random();
            for (int i = 0; i < 100; i++)
            {
                int r = random.Next(0, 1000);
                var style = cells[r, 0].GetDisplayStyle();
                Console.WriteLine($"Cell ({r},0) style: {style.ForegroundArgbColor:X}");
            }

            // Закройте кэш доступа
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


