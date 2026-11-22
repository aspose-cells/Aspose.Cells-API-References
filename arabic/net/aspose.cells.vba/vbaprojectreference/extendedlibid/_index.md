---
title: "VbaProjectReference.ExtendedLibid"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProjectReference. تحصل وتضبط Libid الموسع للإشارة"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreference/extendedlibid/
---
## VbaProjectReference.ExtendedLibid property

يحصل ويضبط Libid الموسع للمرجع.

```csharp
public string ExtendedLibid { get; set; }
```

### ملاحظات

فقط لإشارة التحكم.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferencePropertyExtendedLibidDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // تهيئة مشروع VBA
                VbaProject vbaProject = workbook.VbaProject;

                // إضافة إشارة تحكم لعرض ExtendedLibid
                vbaProject.References.AddControlRefrernce(
                    "SampleControl",
                    "{00020430-0000-0000-C000-000000000046}",
                    "stdole2.tlb",
                    "2.0");

                // الحصول على الإشارة الأولى
                VbaProjectReference reference = vbaProject.References[0];

                // عرض قيمة خاصية ExtendedLibid
                Console.WriteLine("ExtendedLibid value: " + reference.ExtendedLibid);

                // عرض ضبط ExtendedLibid (نظرًا لأنه قابل للقراءة والكتابة)
                reference.ExtendedLibid = "3.0";
                Console.WriteLine("Updated ExtendedLibid value: " + reference.ExtendedLibid);

                // احفظ المصنف
                workbook.Save("ExtendedLibidDemo.xlsm");
                Console.WriteLine("Workbook saved successfully with ExtendedLibid demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


