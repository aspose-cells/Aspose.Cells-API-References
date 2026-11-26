---
title: "Outline.SummaryRowBelow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Outline. Указывает, будет ли строка итога расположена ниже строк деталей в структуре"
type: docs
url: /ru/net/aspose.cells/outline/summaryrowbelow/
---
## Outline.SummaryRowBelow property

Указывает, будет ли строка итогов размещена ниже строк деталей в outline.

```csharp
public bool SummaryRowBelow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryRowBelowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные и группировку
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");
            
            // Группировать строки и установить положение строки итога
            worksheet.Cells.GroupRows(1, 2, false);
            Outline outline = worksheet.Outline;
            outline.SummaryRowBelow = true;
            
            workbook.Save("OutlineSummaryRowBelow.xlsx");
        }
    }
}
```

### См. также

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


