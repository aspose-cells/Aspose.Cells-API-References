---
title: "ReferredArea.SheetName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReferredArea. Указывает, в каком листе находится эта ссылка"
type: docs
url: /ru/net/aspose.cells/referredarea/sheetname/
---
## ReferredArea.SheetName property

Указывает, в каком листе находится эта ссылка.

```csharp
public string SheetName { get; }
```

### Примечания

Если ссылка относится к нескольким листам, возвращаемое значение выглядит как выражение диапазона в формуле. Например, "Sheet1:Sheet3" для ссылки в формуле "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertySheetNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            Worksheet worksheet1 = workbook.Worksheets["Sheet1"];
            
            workbook.Worksheets["Sheet2"].Cells.CreateRange("E5:I6").Name = "someNamedRange_1";
            worksheet1.Cells["A1"].Formula = "=SUM(someNamedRange_1)";
            
            ReferredArea ra = worksheet1.Cells["A1"].GetPrecedents()[0];
            Console.WriteLine("Precedent's referred sheet: " + ra.SheetName);
        }
    }
}
```

### См. также

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


