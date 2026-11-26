---
title: "ReferredArea.EndRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReferredArea. Конечная строка области"
type: docs
url: /ru/net/aspose.cells/referredarea/endrow/
---
## ReferredArea.EndRow property

Конечная строка области.

```csharp
public int EndRow { get; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyEndRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Установить формулу с несколькими ссылками
            cells["A1"].Formula = "= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1";
            
            // Получить все предшествующие области
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Обработать каждую ссылку
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                
                // Продемонстрировать использование EndRow для диапазонных ссылок
                if (area.IsArea)
                {
                    sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
                }
                
                Console.WriteLine(sb.ToString());
            }
            
            workbook.Save("ReferredAreaExample.xlsx");
        }
    }
}
```

### См. также

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


