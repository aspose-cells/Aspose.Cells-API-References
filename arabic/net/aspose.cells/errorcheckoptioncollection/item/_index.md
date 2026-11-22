---
title: "ErrorCheckOptionCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ErrorCheckOptionCollection. تحصل على كائن ErrorCheckOption بواسطة الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/errorcheckoptioncollection/item/
---
## ErrorCheckOptionCollection indexer

يحصل على كائن [`ErrorCheckOption`](../../errorcheckoption/) بواسطة الفهرس المحدد.

```csharp
public ErrorCheckOption this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس |

### قيمة الإرجاع

إرجاع كائن [`ErrorCheckOption`](../../errorcheckoption/)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;
            int optionIdx = opts.Add();
            
            // عرض استخدام خاصية Item
            ErrorCheckOption opt = opts[optionIdx];
            
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.AddRange(CellArea.CreateCellArea("A1", "B3"));

            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


