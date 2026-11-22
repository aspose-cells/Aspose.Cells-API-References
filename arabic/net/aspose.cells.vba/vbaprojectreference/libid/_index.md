---
title: "VbaProjectReference.Libid"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProjectReference. تحصل وتعيّن Libid للمرجع"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreference/libid/
---
## VbaProjectReference.Libid property

يحصل ويضبط Libid للمرجع.

```csharp
public string Libid { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyLibidDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook targetWorkbook = new Workbook();
            
            // حمّل مصنف المصدر مع مشروع VBA
            Workbook sourceWorkbook = new Workbook("source.xlsm");
            
            // امسح المراجع الحالية في الهدف
            targetWorkbook.VbaProject.References.Clear();
            
            // نسخ المراجع من المصدر إلى الهدف
            foreach (VbaProjectReference reference in sourceWorkbook.VbaProject.References)
            {
                if (reference.Type == VbaProjectReferenceType.Registered)
                {
                    // عرض استخدام خاصية Libid
                    targetWorkbook.VbaProject.References.AddRegisteredReference(reference.Name, reference.Libid);
                }
                else if (reference.Type == VbaProjectReferenceType.Control)
                {
                    targetWorkbook.VbaProject.References.AddControlRefrernce(
                        reference.Name, 
                        reference.Libid, 
                        reference.Twiddledlibid, 
                        reference.ExtendedLibid);
                }
            }
            
            // حفظ النتيجة
            targetWorkbook.Save("output.xlsm");
        }
    }
}
```

### انظر أيضًا

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


