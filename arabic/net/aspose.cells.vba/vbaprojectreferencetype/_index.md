---
title: "التعداد VbaProjectReferenceType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Vba.VbaProjectReferenceType. يمثل نوع مرجع مشروع VBA"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreferencetype/
---
## VbaProjectReferenceType enumeration

يمثل نوع مرجع مشروع VBA.

```csharp
public enum VbaProjectReferenceType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Registered | `0` | يحدد مرجعًا إلى مكتبة نوع الأتمتة. |
| Control | `1` | يحدد مرجعًا إلى مكتبة نوع معدلة ومكتبة النوع الموسعة الخاصة بها. |
| Project | `2` | يحدد مرجعًا إلى مشروع VBA خارجي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferenceTypeDemo
    {
        public static void VbaProjectReferenceTypeExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // تهيئة مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;

            // إضافة مرجع مشروع VBA
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // حفظ ملف Excel
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");

            // عرض استخدام تعداد VbaProjectReferenceType
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


