---
title: "VbaProjectReferenceCollection.AddControlRefrernce"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaProjectReferenceCollection. إضافة إشارة إلى مكتبة نوع مُعدَّلة ومكتبة النوع الموسعة الخاصة بها"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/
---
## VbaProjectReferenceCollection.AddControlRefrernce method

أضف مرجعًا إلى مكتبة نوع مُعدلة ومكتبة النوع الموسعة الخاصة بها.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddControlReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddControlRefrernce(string name, string libid, string twiddledlibid, 
    string extendedLibid)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الإشارة. |
| libid | String | معرف مكتبة نوع Automation. |
| twiddledlibid | String | معرف مكتبة نوع مُعدَّلة |
| extendedLibid | String | معرف مكتبة نوع موسعة |

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة VbaProjectReferenceCollection.AddControlReferernce(). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddControlRefrernceWithStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            // إضافة إشارة تحكم مع جميع معلمات السلسلة.
            vbaProject.References.AddControlRefrernce(
                "MSForms",
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library",
                "twiddledLibid",
                "extendedLibid");

            Console.WriteLine("Control reference added successfully. Total references: " + vbaProject.References.Count);
            
            workbook.Save("VbaProjectWithControlReference.xlsm");
        }
    }
}
```

### انظر أيضًا

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


