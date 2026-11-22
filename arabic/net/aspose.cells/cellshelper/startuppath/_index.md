---
title: "CellsHelper.StartupPath"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsHelper. تحصل أو تعيين مسار بدء التشغيل الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية"
type: docs
url: /ar/net/aspose.cells/cellshelper/startuppath/
---
## CellsHelper.StartupPath property

يحصل أو يعيّن مسار بدء التشغيل، الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية.

```csharp
public static string StartupPath { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyStartupPathDemo
    {
        public static void Run()
        {
            // تعيين مسار بدء التشغيل
            CellsHelper.StartupPath = "C:\\Temp\\AsposeCellsStartup";
            
            // عرض مسار بدء التشغيل
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);

            // عرض خصائص CellsHelper الإضافية
            CellsHelper.SignificantDigits = 15;
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


