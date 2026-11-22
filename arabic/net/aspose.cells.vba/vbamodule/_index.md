---
title: "الفئة VbaModule"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Vba.VbaModule class. يمثل الوحدة في مشروع VBA"
type: docs
url: /ar/net/aspose.cells.vba/vbamodule/
---
## VbaModule class

يمثل الوحدة في مشروع VBA.

```csharp
public class VbaModule
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BinaryCodes](../../aspose.cells.vba/vbamodule/binarycodes/) { get; } | يسترجع ويضبط الرموز الثنائية للوحدة. |
| [Codes](../../aspose.cells.vba/vbamodule/codes/) { get; set; } | يسترجع ويضبط رموز الوحدة. |
| [Name](../../aspose.cells.vba/vbamodule/name/) { get; set; } | يسترجع ويضبط اسم الوحدة. |
| [Type](../../aspose.cells.vba/vbamodule/type/) { get; } | يسترجع نوع الوحدة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleDemo
    {
        public static void VbaModuleExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // تهيئة مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;

            // إضافة وحدة جديدة
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");

            // الحصول على وحدة VBA
            VbaModule vbaModule = vbaProject.Modules[index];

            // تعيين الرموز للوحدة
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";

            // حفظ ملف Excel
            workbook.Save("VbaModuleExample.xlsm");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


