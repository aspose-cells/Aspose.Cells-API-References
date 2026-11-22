---
title: "VbaProjectReferenceCollection.AddRegisteredReference"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaProjectReferenceCollection. أضف مرجعًا إلى مكتبة نوع Automation"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/
---
## VbaProjectReferenceCollection.AddRegisteredReference method

أضف مرجعًا إلى مكتبة نوع الأتمتة.

```csharp
public int AddRegisteredReference(string name, string libid)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الإشارة. |
| libid | String | معرف مكتبة نوع Automation. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddRegisteredReferenceWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // أضف مرجعًا مسجلاً إلى stdole
            vbaProject.References.AddRegisteredReference(
                "stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // احفظ المصنف
            workbook.Save("output.xlsm");
        }
    }
}
```

### انظر أيضًا

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


