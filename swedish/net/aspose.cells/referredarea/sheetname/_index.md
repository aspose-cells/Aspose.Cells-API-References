---
title: "ReferredArea.SheetName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReferredArea-egenskap. Anger vilket blad denna referens finns i"
type: docs
url: /sv/net/aspose.cells/referredarea/sheetname/
---
## ReferredArea.SheetName property

Indikerar vilket blad denna referens finns i.

```csharp
public string SheetName { get; }
```

### Anmärkningar

Om den refererar till flera arbetsblad är det returnerade värdet precis som områdesuttrycket i formeln. Till exempel "Sheet1:Sheet3" för referensen i formeln "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

### Exempel

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

### Se även

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


