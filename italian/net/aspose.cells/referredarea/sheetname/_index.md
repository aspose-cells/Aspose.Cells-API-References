---
title: "ReferredArea.SheetName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReferredArea. Indica in quale foglio si trova questo riferimento"
type: docs
url: /it/net/aspose.cells/referredarea/sheetname/
---
## ReferredArea.SheetName property

Indica in quale foglio si trova questo riferimento.

```csharp
public string SheetName { get; }
```

### Osservazioni

Se fa riferimento a più fogli di lavoro, il valore restituito è proprio come l'espressione di intervallo nella formula. Per esempio "Sheet1:Sheet3" per il riferimento nella formula "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

### Esempi

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

### Vedi anche

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


