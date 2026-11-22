---
title: "DocumentPropertyCollection.Contains"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DocumentPropertyCollection. تُرجع true إذا كانت خاصية بالاسم المحدد موجودة في المجموعة"
type: docs
url: /ar/net/aspose.cells.properties/documentpropertycollection/contains/
---
## DocumentPropertyCollection.Contains method

يعيد true إذا كانت خاصية بالاسم المحدد موجودة في المجموعة.

```csharp
public bool Contains(string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية غير حساس لحالة الأحرف. |

### قيمة الإرجاع

true إذا كانت الخاصية موجودة في المجموعة؛ false خلاف ذلك.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionMethodContainsWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تحقق مما إذا كانت خاصية "RevisionNumber" موجودة في خصائص المستند المدمجة
            bool containsRevision = workbook.BuiltInDocumentProperties.Contains("RevisionNumber");
            Console.WriteLine("Contains 'RevisionNumber': " + containsRevision);
            
            // أضف خاصية مخصصة وتحقق من وجودها
            workbook.CustomDocumentProperties.Add("CustomProperty", "Test Value");
            bool containsCustom = workbook.CustomDocumentProperties.Contains("CustomProperty");
            Console.WriteLine("Contains 'CustomProperty': " + containsCustom);
        }
    }
}
```

### انظر أيضًا

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


