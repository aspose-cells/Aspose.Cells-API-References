---
title: "ErrorCheckOption.AddRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ErrorCheckOption. تضيف نطاقًا واحدًا متأثرًا بهذا الإعداد"
type: docs
url: /ar/net/aspose.cells/errorcheckoption/addrange/
---
## ErrorCheckOption.AddRange method

يضيف نطاقًا واحدًا متأثرًا بهذا الإعداد.

```csharp
public int AddRange(CellArea ca)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | CellArea | النطاق الذي سيتم إضافته. |

### قيمة الإرجاع

فهرس النطاق المضاف في قائمة النطاقات لهذا الإعداد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodAddRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;
            int index = optsCollection.Add();
            ErrorCheckOption opts = optsCollection[index];
            
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            
            // إضافة نطاقات باستخدام CellArea
            opts.AddRange(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 3 }); // A1:D2
            opts.AddRange(new CellArea { StartRow = 2, StartColumn = 0, EndRow = 2, EndColumn = 3 }); // A3:D3
            
            // احفظ المصنف
            workbook.Save("ErrorCheckOptionMethodAddRangeWithCellAreaDemo.xls");
            
            Console.WriteLine("Workbook saved with error check options.");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


