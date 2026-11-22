---
title: "NameCollection.RemoveDuplicateNames"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة NameCollection. إزالة الأسماء المعرفة المكررة"
type: docs
url: /ar/net/aspose.cells/namecollection/removeduplicatenames/
---
## NameCollection.RemoveDuplicateNames method

إزالة الأسماء المعرفة المكررة

```csharp
public void RemoveDuplicateNames()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveDuplicateNamesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض النطاقات المسماة بأسماء مكررة
            worksheet.Cells["A1"].PutValue("Test Value 1");
            worksheet.Cells["B1"].PutValue("Test Value 2");
            
            // إنشاء نطاقات مسماة مكررة باستخدام توقيع طريقة Add الصحيح
            int index1 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$B$1";
            
            // عرض العدد قبل إزالة التكرارات
            Console.WriteLine($"Named ranges count before removal: {workbook.Worksheets.Names.Count}");
            
            // إزالة الأسماء المكررة
            workbook.Worksheets.Names.RemoveDuplicateNames();
            
            // عرض العدد بعد إزالة التكرارات
            Console.WriteLine($"Named ranges count after removal: {workbook.Worksheets.Names.Count}");
        }
    }
}
```

### انظر أيضًا

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


