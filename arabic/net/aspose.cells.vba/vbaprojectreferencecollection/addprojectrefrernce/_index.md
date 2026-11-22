---
title: "VbaProjectReferenceCollection.AddProjectRefrernce"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaProjectReferenceCollection. يضيف إشارة إلى مشروع VBA خارجي"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/
---
## VbaProjectReferenceCollection.AddProjectRefrernce method

يضيف مرجعًا إلى مشروع VBA خارجي.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddProjectReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddProjectRefrernce(string name, string absoluteLibid, string relativeLibid)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الإشارة. |
| absoluteLibid | String | معرف مشروع VBA المشار إليه مع مسار مطلق. |
| relativeLibid | String | معرف مشروع VBA المشار إليه مع مسار نسبي. |

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة VbaProjectReferenceCollection.AddProjectReferernce(). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddProjectRefrernceWithStringStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تهيئة مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // إضافة إشارة مشروع مع libids مطلق ونسبي
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // عرض عدد الإشارات
            Console.WriteLine("Total References: " + vbaProject.References.Count);
            
            // احفظ المصنف
            workbook.Save("VbaProjectReferenceExample.xlsm");
        }
    }
}
```

### انظر أيضًا

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


