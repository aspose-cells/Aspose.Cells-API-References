---
title: "VbaProject.IslockedForViewing"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProject. تشير إلى ما إذا كان مشروع VBA هذا مقفلًا للعرض"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/islockedforviewing/
---
## VbaProject.IslockedForViewing property

تشير إلى ما إذا كان مشروع VBA هذا مقفلًا للعرض.

```csharp
[Obsolete("Use VbaProject.IsLockedForView property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IslockedForViewing { get; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية VbaProject.IsLockedForView. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIslockedForViewingDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا تجريبيًا مع مشروع VBA
            Workbook wb = new Workbook();
            // إنشاء ورقة عمل جديدة لضمان إنشاء مشروع VBA
            wb.Worksheets.Add();
            
            // عرض خاصية IslockedForViewing
            Console.WriteLine("Initial state:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // حماية وقفل للعرض
            wb.VbaProject.Protect(true, "password123");
            Console.WriteLine("After protecting and locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // حماية دون قفل للعرض
            wb.VbaProject.Protect(false, "password456");
            Console.WriteLine("After protecting without locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // إزالة الحماية
            wb.VbaProject.Protect(true, "");
            Console.WriteLine("After removing protection:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}");
        }
    }
}
```

### انظر أيضًا

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


