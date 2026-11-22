---
title: "WorksheetCollection.Names"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تحصل على مجموعة جميع كائنات Name في جدول البيانات"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/names/
---
## WorksheetCollection.Names property

يحصل على مجموعة جميع كائنات Name في جدول البيانات.

```csharp
public NameCollection Names { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyNamesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل بأحرف خاصة في الاسم
            Worksheet worksheet = workbook.Worksheets.Add("My.Test");
            
            // الوصول إلى مجموعة Names
            NameCollection names = workbook.Worksheets.Names;
            
            // إضافة نطاق مسمى جديد
            int index = names.Add("My.Test!TestName");
            Name namedRange = names[index];
            
            // تعيين مرجع النطاق وتوضيح الاستخدام
            namedRange.RefersTo = "=My.Test!$A$1:$B$2";
            
            // إخراج خصائص النطاق المسمى
            Console.WriteLine("Name: " + namedRange.Text);
            Console.WriteLine("FullText: " + namedRange.FullText);
            Console.WriteLine("RefersTo: " + namedRange.RefersTo);
        }
    }
}
```

### انظر أيضًا

* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


