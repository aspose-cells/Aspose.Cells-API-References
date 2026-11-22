---
title: "CellsHelper.AltStartPath"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsHelper. يحصل أو يضبط مسار بدء التشغيل البديل الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية"
type: docs
url: /ar/net/aspose.cells/cellshelper/altstartpath/
---
## CellsHelper.AltStartPath property

يحصل أو يعيّن مسار بدء التشغيل البديل، الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية.

```csharp
public static string AltStartPath { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyAltStartPathDemo
    {
        public static void Run()
        {
            // ضبط مسار بدء التشغيل البديل
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            
            // قم أيضًا بضبط خصائص أخرى ذات صلة للتوضيح
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            
            // اعرض المسارات لتوضيح استخدام الخاصية
            Console.WriteLine("Main Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            
            // مثال على كيفية استخدام هذه المسارات
            Console.WriteLine("\nWhen resources aren't found in main path, system will check: " + CellsHelper.AltStartPath);
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


