---
title: "VbaModule.Codes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaModule. يحصل على ويضبط رموز الوحدة"
type: docs
url: /ar/net/aspose.cells.vba/vbamodule/codes/
---
## VbaModule.Codes property

يسترجع ويضبط رموز الوحدة.

```csharp
public string Codes { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyCodesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف وحدة VBA
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            Aspose.Cells.Vba.VbaModule module = workbook.VbaProject.Modules[index];
            
            // حدد الكود الأولي
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello World\"\nEnd Sub";
            
            // عدّل الكود بإضافة أسطر جديدة
            module.Codes = module.Codes + "\nSub AnotherMacro()\n    MsgBox \"Second Macro\"\nEnd Sub";
            
            // احفظ المصنف
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### انظر أيضًا

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


