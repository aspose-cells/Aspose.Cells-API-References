---
title: "VbaProjectReference.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProjectReference. تحصل على نوع هذه الإشارة"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreference/type/
---
## VbaProjectReference.Type property

يحصل على نوع هذا المرجع.

```csharp
public VbaProjectReferenceType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // تهيئة مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;

            // إضافة إشارة مسجلة إلى مشروع VBA
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // الحصول على الإشارة الأولى وعرض خاصية Type
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);

            // احفظ المصنف
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");
        }
    }
}
```

### انظر أيضًا

* enum [VbaProjectReferenceType](../../vbaprojectreferencetype/)
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


