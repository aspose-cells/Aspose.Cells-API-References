---
title: "NameCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية NameCollection. تحصل على عنصر Name في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/namecollection/item/
---
## NameCollection indexer (1 of 2)

يحصل على عنصر [`Name`](../../name/) في الفهرس المحدد.

```csharp
public Name this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض أوراق العمل
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // الوصول إلى مجموعة الأسماء
            NameCollection names = workbook.Worksheets.Names;
            
            // إضافة نطاقات مسماة باستخدام توقيع الطريقة الصحيح
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$B$2";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet2!$C$3:$D$4";
            
            int index3 = names.Add("Range3");
            names[index3].RefersTo = "=Sheet3!$E$5:$F$6";

            // عرض استخدام خاصية Item
            Console.WriteLine("Named Ranges:");
            for (int i = 0; i < names.Count; i++)
            {
                Name name = names[i]; // Using Item property with index
                Console.WriteLine($"{name.Text}: {name.RefersTo}");
            }

            // الوصول بالاسم باستخدام خاصية Item
            Name specificName = names["Range2"];
            Console.WriteLine($"\nSpecific Range: {specificName.Text} refers to {specificName.RefersTo}");

            // تعديل نطاق مسمى
            names["Range3"].RefersTo = "=Sheet3!$A$1:$B$10";
            Console.WriteLine($"\nModified Range3 now refers to: {names["Range3"].RefersTo}");
        }
    }
}
```

### انظر أيضًا

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## NameCollection indexer (2 of 2)

يحصل على عنصر [`Name`](../../name/) بالاسم المحدد.

```csharp
public Name this[string text] { get; }
```

| معامل | الوصف |
| --- | --- |
| نص | نص الاسم. |

### قيمة الإرجاع

العنصر بالاسم المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى مجموعة أسماء أوراق العمل
            NameCollection names = workbook.Worksheets.Names;
            
            // إضافة بعض النطاقات المسماة (تم التصحيح لاستخدام توقيع طريقة Add الصحيح)
            int index1 = names.Add("Range1");
            names[index1].RefersTo = "=Sheet1!$A$1:$A$10";
            
            int index2 = names.Add("Range2");
            names[index2].RefersTo = "=Sheet1!$B$1:$B$10";
            
            // الوصول إلى النطاقات المسماة باستخدام خاصية Item
            Name range1 = names["Range1"];
            Name range2 = names["Range2"];
            
            // تحقق من وجود الأسماء
            if (range1 != null && range2 != null)
            {
                Console.WriteLine("Named range 'Range1' refers to: " + range1.RefersTo);
                Console.WriteLine("Named range 'Range2' refers to: " + range2.RefersTo);
            }
            
            // حاول الوصول إلى اسم غير موجود
            Name range3 = names["NonExistentRange"];
            if (range3 == null)
            {
                Console.WriteLine("Named range 'NonExistentRange' not found");
            }
        }
    }
}
```

### انظر أيضًا

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


