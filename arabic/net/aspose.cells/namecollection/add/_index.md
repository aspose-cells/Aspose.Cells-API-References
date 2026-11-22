---
title: "NameCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة NameCollection. تُعرّف اسمًا جديدًا"
type: docs
url: /ar/net/aspose.cells/namecollection/add/
---
## NameCollection.Add method

يعرف اسمًا جديدًا.

```csharp
public int Add(string text)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | النص لاستخدامه كاسم. |

### قيمة الإرجاع

[`Name`](../../name/) object index.

### ملاحظات

لا يمكن أن يحتوي الاسم على مسافات ولا يمكن أن يشبه مراجع الخلايا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = wb.Worksheets[0];
            
            // إضافة اسم مع مرجع نصي
            int index = wb.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = wb.Worksheets.Names[index];
            
            // ضبط الصيغة التي يشير إليها الاسم
            namedRange.RefersTo = "=Sheet1!$A$1:$B$10";
            
            // التحقق وإخراج النتائج
            Console.WriteLine("Named Range RefersTo: " + namedRange.RefersTo);
            Console.WriteLine("Named Range Index: " + index);
            
            // الحصول على النطاق وعرض عنوانه
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Range Address: " + range.Address);
        }
    }
}
```

### انظر أيضًا

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


