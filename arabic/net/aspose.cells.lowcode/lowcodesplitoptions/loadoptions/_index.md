---
title: "LowCodeSplitOptions.LoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSplitOptions. خيارات التحميل لتحميل جدول البيانات الذي سيتم تقسيمه"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesplitoptions/loadoptions/
---
## LowCodeSplitOptions.LoadOptions property

خيارات التحميل لتحميل جدول البيانات الذي سيتم تقسيمه.

```csharp
public LowCodeLoadOptions LoadOptions { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertyLoadOptionsDemo
    {
        public static void Run()
        {
            // إنشاء كائن خيارات التقسيم
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // تهيئة خيارات التحميل
            splitOptions.LoadOptions = new LowCodeLoadOptions();

            // إنشاء خيارات تحميل جديدة بإعدادات مختلفة (باستخدام الخصائص المتاحة)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // عرض التكوين النهائي
            Console.WriteLine("LoadOptions configured with InputFile: " + splitOptions.LoadOptions.InputFile);
        }
    }
}
```

### انظر أيضًا

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


