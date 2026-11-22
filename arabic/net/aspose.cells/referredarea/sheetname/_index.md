---
title: "ReferredArea.SheetName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReferredArea. تشير إلى الورقة التي توجد فيها هذه الإشارة"
type: docs
url: /ar/net/aspose.cells/referredarea/sheetname/
---
## ReferredArea.SheetName property

يشير إلى الورقة التي توجد فيها هذه الإشارة.

```csharp
public string SheetName { get; }
```

### ملاحظات

إذا كان يشير إلى عدة أوراق عمل، فإن القيمة المرجعة تكون مشابهة لتعبير النطاق في الصيغة. على سبيل المثال \"Sheet1:Sheet3\" للإشارة في الصيغة \"=SUM(Sheet1:Sheet3!$A$1:$B$2)\".

### أمثلة

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

### انظر أيضًا

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


