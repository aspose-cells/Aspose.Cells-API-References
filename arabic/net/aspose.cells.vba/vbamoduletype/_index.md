---
title: "التعداد VbaModuleType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Vba.VbaModuleType. يمثل نوع وحدة VBA"
type: docs
url: /ar/net/aspose.cells.vba/vbamoduletype/
---
## VbaModuleType enumeration

يمثل نوع وحدة VBA.

```csharp
public enum VbaModuleType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Procedural | `0` | يمثل وحدة إجرائية. |
| Document | `1` | يمثل وحدة مستند. |
| Class | `2` | يمثل وحدة فئة. |
| Designer | `3` | يمثل وحدة مصمم. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleTypeDemo
    {
        public static void VbaModuleTypeExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            
            // تهيئة مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // إضافة وحدة فئة جديدة
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
            
            // الحصول على وحدة VBA
            VbaModule vbaModule = vbaProject.Modules[index];
            
            // تعيين الرموز للوحدة
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
            
            // احفظ ملف Excel
            workbook.Save("VbaModuleTypeExample.xlsm");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


