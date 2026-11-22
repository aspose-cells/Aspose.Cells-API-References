---
title: "الفئة ProtectedRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.ProtectedRange فئة. نطاق محدد يُسمح بتحريره عندما تكون حماية الورقة مفعلة"
type: docs
url: /ar/net/aspose.cells/protectedrange/
---
## ProtectedRange class

نطاق محدد يُسمح بتحريره عندما تكون حماية الورقة مفعلة.

```csharp
public class ProtectedRange
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CellArea](../../aspose.cells/protectedrange/cellarea/) { get; } | يحصل على الكائن [`CellArea`](./cellarea/) الذي يمثل مساحة الخلية التي سيتم حمايتها. |
| [IsProtectedWithPassword](../../aspose.cells/protectedrange/isprotectedwithpassword/) { get; } | يشير إلى ما إذا كانت أوراق العمل محمية بكلمة مرور. |
| [Name](../../aspose.cells/protectedrange/name/) { get; set; } | يحصل على عنوان النطاق. يُستخدم هذا كواصف، وليس كتعريف نطاق مسمى. |
| [Password](../../aspose.cells/protectedrange/password/) { get; set; } | يمثل كلمة المرور لحماية النطاق. |
| [SecurityDescriptor](../../aspose.cells/protectedrange/securitydescriptor/) { get; set; } | محدد الأمان يحدد حسابات المستخدمين الذين يمكنهم تحرير هذا النطاق دون تقديم كلمة مرور للوصول إلى النطاق. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddArea](../../aspose.cells/protectedrange/addarea/)(int, int, int, int) | يضيف مساحة مُشار إليها إلى هذا |
| [GetAreas](../../aspose.cells/protectedrange/getareas/)() | يحصل على جميع المساحات المُشار إليها. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectedRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على مجموعة النطاقات المحمية
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // أضف نطاقًا محميًا جديدًا (A1:J10)
            int index = protectedRanges.Add("MyProtectedRange", 0, 0, 10, 10);
            
            // احصل على النطاق المحمي
            ProtectedRange protectedRange = protectedRanges[index];
            
            // تعيين محدد الأمان
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            protectedRange.SecurityDescriptor = securityDescriptor;
            
            // احفظ المصنف
            workbook.Save("ProtectedRangeDemo.xlsx");
            
            Console.WriteLine("Protected range demo completed successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


