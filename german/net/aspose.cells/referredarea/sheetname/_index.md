---
title: "ReferredArea.SheetName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReferredArea-Eigenschaft. Gibt an, in welchem Blatt diese Referenz liegt"
type: docs
url: /de/net/aspose.cells/referredarea/sheetname/
---
## ReferredArea.SheetName property

Gibt an, in welchem Blatt diese Referenz ist.

```csharp
public string SheetName { get; }
```

### Hinweise

Wenn es auf mehrere Arbeitsblätter verweist, entspricht der zurückgegebene Wert dem Bereichsausdruck in der Formel. Zum Beispiel "Sheet1:Sheet3" für die Referenz in der Formel "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

### Beispiele

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

### Siehe auch

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


