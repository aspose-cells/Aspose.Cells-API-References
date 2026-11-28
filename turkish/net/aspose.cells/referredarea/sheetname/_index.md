---
title: "ReferredArea.SheetName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReferredArea özelliği. Bu başvurunun hangi sayfada olduğunu gösterir."
type: docs
url: /tr/net/aspose.cells/referredarea/sheetname/
---
## ReferredArea.SheetName property

Bu referansın hangi sayfada olduğunu gösterir.

```csharp
public string SheetName { get; }
```

### Açıklamalar

Birden fazla çalışma sayfasına başvuruyorsa, döndürülen değer formüldeki aralık ifadesi gibi olur. Örneğin "Sheet1:Sheet3" ifadesi, "=SUM(Sheet1:Sheet3!$A$1:$B$2)" formülündeki başvuru için.

### Örnekler

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

### Ayrıca Bakınız

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


