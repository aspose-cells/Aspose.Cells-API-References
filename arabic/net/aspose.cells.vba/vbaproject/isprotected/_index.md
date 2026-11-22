---
title: "VbaProject.IsProtected"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProject. تشير إلى ما إذا كان مشروع VBA هذا محميًا"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/isprotected/
---
## VbaProject.IsProtected property

يشير إلى ما إذا كان مشروع VBA هذا محميًا.

```csharp
public bool IsProtected { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // تحميل ملف Excel تجريبي يحتوي على مشروع VBA غير محمي
            Workbook wb = new Workbook("load.xlsm");
            VbaProject vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // تحميل ملف Excel تجريبي يحتوي على مشروع VBA محمي
            wb = new Workbook("load_protected.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // تحميل ملف Excel تجريبي يحتوي على مشروع VBA محمي ومقفل
            wb = new Workbook("load_protected_lockedForView.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected_lockedForView.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);
        }
    }
}
```

### انظر أيضًا

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


