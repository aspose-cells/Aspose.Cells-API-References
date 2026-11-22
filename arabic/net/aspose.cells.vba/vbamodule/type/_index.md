---
title: "VbaModule.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaModule. يحصل على نوع الوحدة"
type: docs
url: /ar/net/aspose.cells.vba/vbamodule/type/
---
## VbaModule.Type property

يسترجع نوع الوحدة.

```csharp
public VbaModuleType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyTypeDemo
    {
        public static void Run()
        {
            // أنشئ دفتر عمل مع ملف ماكرو مفعّل تجريبي
            Workbook wb = new Workbook("example.xlsm");
            
            // الوصول إلى مشروع VBA والوحدات
            VbaProject vbaProject = wb.VbaProject;
            VbaModuleCollection modules = vbaProject.Modules;
            
            // اعرض أنواع الوحدات وأسمائها
            for (int i = 0; i < modules.Count; i++)
            {
                Console.WriteLine($"Module Name: {modules[i].Name}");
                Console.WriteLine($"Module Type: {modules[i].Type}");
                Console.WriteLine();
            }
            
            wb.Save("output.xlsm");
        }
    }
}
```

### انظر أيضًا

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


