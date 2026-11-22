---
title: "VbaProject.References"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProject. تحصل على جميع المراجع لمشروع VBA"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/references/
---
## VbaProject.References property

يحصل على جميع مراجع مشروع VBA.

```csharp
public VbaProjectReferenceCollection References { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyReferencesDemo
    {
        public static void Run()
        {
            // إنشاء مصنف (يتم إنشاء مشروع VBA تلقائيًا لملفات .xlsm)
            Workbook workbook = new Workbook();
            
            // الوصول إلى مراجع مشروع VBA (متاح فقط إذا كان المصنف يحتوي على مشروع VBA)
            if (workbook.VbaProject != null)
            {
                VbaProjectReferenceCollection references = workbook.VbaProject.References;
                
                // إضافة أنواع مختلفة من المراجع
                references.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
                references.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "", "");
                references.AddProjectRefrernce("MyProject", "C:\\Projects\\MyProject.xlam", "..\\MyProject.xlam");

                // عرض عدد الإشارات
                Console.WriteLine($"Total references: {references.Count}");
            }

            // حفظ كدفتر عمل يدعم الماكرو
            workbook.Save("VbaProjectWithReferences.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### انظر أيضًا

* class [VbaProjectReferenceCollection](../../vbaprojectreferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


