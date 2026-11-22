---
title: "VbaProject.Modules"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProject. يحصل على جميع كائنات VbaModule"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/modules/
---
## VbaProject.Modules property

يحصل على جميع كائنات [`VbaModule`](../../vbamodule/).

```csharp
public VbaModuleCollection Modules { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyModulesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;
            
            // أضف وحدة جديدة واحصل عليها باستخدام خاصية Modules
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            
            // أضف كودًا إلى الوحدة
            module.Codes = "Sub Test()\r\n    MsgBox \"Module demonstration\"\r\nEnd Sub";
            
            // احفظ بصيغة تدعم الماكرو
            workbook.Save("VbaModulesDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### انظر أيضًا

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


