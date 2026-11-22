---
title: "NameCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة NameCollection. إزالة الاسم عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/namecollection/removeat/
---
## NameCollection.RemoveAt method

إزالة الاسم في الفهرس المحدد.

```csharp
public void RemoveAt(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس الاسم المراد إزالته. |

### ملاحظات

يرجى التأكد من أن الاسم غير مُشار إليه من قبل الصيغ الأخرى قبل استدعاء الطريقة. وإذا كان الاسم مُشارًا إليه، فإن ضبط Name.RefersTo كقيمة null يكون أفضل.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;
            NameCollection names = worksheets.Names;

            // إضافة أسماء إلى المجموعة
            int firstIndex = names.Add("FirstRange");
            names[firstIndex].RefersTo = "=Sheet1!$A$1:$A$5";
            
            int secondIndex = names.Add("SecondRange");
            names[secondIndex].RefersTo = "=Sheet1!$B$1:$B$5";

            // إزالة الاسم حسب الفهرس
            names.RemoveAt(firstIndex);

            // تحقق من الإزالة عن طريق فحص العدد
            Console.WriteLine($"Remaining names count: {names.Count}");

            workbook.Save("NameCollectionRemoveAtExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


