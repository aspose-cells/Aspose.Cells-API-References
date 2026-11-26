---
title: "Cell.GetPrecedents"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает все ссылки, появляющиеся в формуле этой ячейки"
type: docs
url: /ru/net/aspose.cells/cell/getprecedents/
---
## Cell.GetPrecedents method

Получает все ссылки, появляющиеся в формуле этой ячейки.

```csharp
public ReferredAreaCollection GetPrecedents()
```

### Возвращаемое значение

Коллекция всех ссылок, появляющихся в формуле этой ячейки.

### Примечания

Возвращает null, если это не ячейка с формулой. Все ссылки, появляющиеся в формуле этой ячейки, будут возвращены независимо от того, используются они при вычислении или нет. Например, хотя ячейка A2 в формуле "=IF(TRUE,A1,A2)" не используется при вычислении, она всё равно считается предшественником формулы. Чтобы получить только те ссылки, которые влияют на вычисление, пожалуйста, используйте [`GetPrecedentsInCalculation`](../getprecedentsincalculation/).

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Установить формулу с предшественниками
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1";
            
            // Получить все ссылки‑предшественники
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Отобразить каждую ссылку‑предшественник
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                if (area.IsArea)
                {
                    sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
                }
                Console.WriteLine(sb.ToString());
            }
        }
    }
}
```

### См. также

* class [ReferredAreaCollection](../../referredareacollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


