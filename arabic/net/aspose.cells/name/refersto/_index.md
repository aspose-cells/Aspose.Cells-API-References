---
title: "Name.RefersTo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Name. تُرجع أو تُعيّن الصيغة التي يُعرّف الاسم للإشارة إليها وتبدأ بعلامة مساواة"
type: docs
url: /ar/net/aspose.cells/name/refersto/
---
## Name.RefersTo property

يعيد أو يضبط الصيغة التي يُعرّف الاسم للإشارة إليها، وتبدأ بعلامة مساواة.

```csharp
public string RefersTo { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyRefersToDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "Sheet1";

            // أضف نطاقات مسماة باستخدام RefersTo
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$6:$8";
            
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$C:$D";

            // اعرض خاصية RefersTo للنطاقات المسماة
            Console.WriteLine("NamedRange1 RefersTo: " + workbook.Worksheets.Names[0].RefersTo);
            Console.WriteLine("NamedRange2 RefersTo: " + workbook.Worksheets.Names[1].RefersTo);
        }
    }
}
```

### انظر أيضًا

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


