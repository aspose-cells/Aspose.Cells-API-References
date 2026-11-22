---
title: "LoadOptions.Password"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحصل وتعيّن كلمة مرور دفتر العمل"
type: docs
url: /ar/net/aspose.cells/loadoptions/password/
---
## LoadOptions.Password property

يحصل على ويضبط كلمة مرور دفتر العمل.

```csharp
public string Password { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // إنشاء خيارات التحميل وتعيين كلمة المرور
            LoadOptions options = new LoadOptions();
            options.Password = "test";

            // تحميل دفتر عمل محمي بكلمة مرور
            Workbook workbook = new Workbook("protected.xlsx", options);

            // إزالة حماية كلمة المرور بعد التحميل
            workbook.Settings.Password = null;

            // حفظ دفتر العمل غير المحمي
            workbook.Save("unprotected.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


