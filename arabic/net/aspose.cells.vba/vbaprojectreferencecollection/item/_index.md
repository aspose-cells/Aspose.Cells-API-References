---
title: "VbaProjectReferenceCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProjectReferenceCollection. احصل على المرجع في القائمة حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreferencecollection/item/
---
## VbaProjectReferenceCollection indexer

احصل على المرجع في القائمة حسب الفهرس.

```csharp
public VbaProjectReference this[int i] { get; }
```

| معامل | الوصف |
| --- | --- |
| i | الفهرس. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تهيئة مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // أضف مراجع إلى مشروع VBA
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            vbaProject.References.AddControlRefrernce("MSForms", 
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", 
                "twiddledLibid", "extendedLibid");
            
            // احصل على مجموعة المراجع
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // الوصول إلى المراجع باستخدام خاصية Item
            VbaProjectReference firstRef = references[0];
            VbaProjectReference secondRef = references[1];
            
            Console.WriteLine("First Reference: " + firstRef.Name);
            Console.WriteLine("Second Reference: " + secondRef.Name);
            
            // احفظ المصنف
            workbook.Save("VbaProjectReferences.xlsm");
        }
    }
}
```

### انظر أيضًا

* class [VbaProjectReference](../../vbaprojectreference/)
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


